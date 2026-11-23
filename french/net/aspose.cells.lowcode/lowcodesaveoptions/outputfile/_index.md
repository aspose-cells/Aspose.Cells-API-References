---
title: "LowCodeSaveOptions.OutputFile"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LowCodeSaveOptions. Obtient et définit le fichier avec le chemin si nécessaire pour enregistrer les données générées. Lors de la définition de cette propriété avec une valeur différente de null ou d'une chaîne vide, OutputStream sera ignoré."
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesaveoptions/outputfile/
---
## LowCodeSaveOptions.OutputFile property

Obtient et définit le fichier (avec le chemin si nécessaire) pour enregistrer les données générées. Lors de la définition de cette propriété avec une valeur différente de null ou d'une chaîne vide, [`OutputStream`](../outputstream/) sera ignoré.

```csharp
public string OutputFile { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeSaveOptionsPropertyOutputFileDemo
    {
        public static void Run()
        {
            // Créer un classeur simple avec une feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // Enregistrer dans différents formats en utilisant la propriété OutputFile
            string outputDir = "Output/";
            Directory.CreateDirectory(outputDir);

            // Enregistrer au format PDF
            SaveWithOutputFile(workbook, SaveFormat.Pdf, "output.pdf");

            // Enregistrer au format JSON
            SaveWithOutputFile(workbook, SaveFormat.Json, "output.json");

            // Enregistrer en tant que HTML
            SaveWithOutputFile(workbook, SaveFormat.Html, "output.html");

            // Enregistrer au format CSV
            SaveWithOutputFile(workbook, SaveFormat.Csv, "output.csv");
        }

        private static void SaveWithOutputFile(Workbook workbook, SaveFormat format, string fileName)
        {
            string outputPath = "Output/" + fileName;
            
            switch (format)
            {
                case SaveFormat.Pdf:
                    PdfConverter.Process(new LowCodeLoadOptions { InputStream = new MemoryStream() },
                        new LowCodePdfSaveOptions { OutputFile = outputPath });
                    break;
                case SaveFormat.Json:
                    JsonConverter.Process(new LowCodeLoadOptions { InputStream = new MemoryStream() },
                        new LowCodeSaveOptions { OutputFile = outputPath });
                    break;
                case SaveFormat.Html:
                    HtmlConverter.Process(new LowCodeLoadOptions { InputStream = new MemoryStream() },
                        new LowCodeSaveOptions { OutputFile = outputPath });
                    break;
                case SaveFormat.Csv:
                    TextConverter.Process(new LowCodeLoadOptions { InputStream = new MemoryStream() },
                        new LowCodeSaveOptions { OutputFile = outputPath });
                    break;
                default:
                    throw new NotSupportedException("Format not supported: " + format);
            }

            Console.WriteLine($"File saved successfully to: {outputPath}");
        }
    }
}
```

### Voir aussi

* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


