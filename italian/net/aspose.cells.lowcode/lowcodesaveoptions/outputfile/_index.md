---
title: "LowCodeSaveOptions.OutputFile"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LowCodeSaveOptions. Ottiene e imposta il file con percorso, se necessario, per salvare i dati generati. Quando si imposta questa proprietà con un valore diverso da null o stringa vuota, OutputStream verrà ignorato"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesaveoptions/outputfile/
---
## LowCodeSaveOptions.OutputFile property

Ottiene e imposta il file (con percorso, se necessario) per salvare i dati generati. Quando si imposta questa proprietà con un valore diverso da null o stringa vuota, [`OutputStream`](../outputstream/) verrà ignorato.

```csharp
public string OutputFile { get; set; }
```

### Esempi

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
            // Crea una cartella di lavoro semplice con un foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // Salva in formati diversi utilizzando la proprietà OutputFile
            string outputDir = "Output/";
            Directory.CreateDirectory(outputDir);

            // Salva come PDF
            SaveWithOutputFile(workbook, SaveFormat.Pdf, "output.pdf");

            // Salva come JSON
            SaveWithOutputFile(workbook, SaveFormat.Json, "output.json");

            // Salva come HTML
            SaveWithOutputFile(workbook, SaveFormat.Html, "output.html");

            // Salva come CSV
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

### Vedi anche

* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


