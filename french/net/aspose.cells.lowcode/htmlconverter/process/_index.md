---
title: "HtmlConverter.Process"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode HtmlConverter. Convertit le fichier modèle donné entre html et d'autres formats"
type: docs
url: /fr/net/aspose.cells.lowcode/htmlconverter/process/
---
## Process(string, string) {#process_1}

Convertit le fichier modèle donné entre le html et d'autres formats.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| templateFile | String | Le fichier modèle à convertir |
| resultFile | String | Le fichier résultant |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class HtmlConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // Créer un fichier HTML temporaire pour la conversion
            string templateFile = CreateSampleHtmlFile();
            string resultFile = "HtmlConversionResult.xlsx";

            try
            {
                // Traiter les fichiers directement en utilisant HtmlConverter
                HtmlConverter.Process(templateFile, resultFile);

                Console.WriteLine($"Successfully converted '{templateFile}' to '{resultFile}'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
            finally
            {
                // Supprimer le fichier temporaire
                if (File.Exists(templateFile))
                {
                    File.Delete(templateFile);
                }
            }
        }

        private static string CreateSampleHtmlFile()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Conversion");
            
            string tempFile = Path.GetTempFileName() + ".html";
            workbook.Save(tempFile, SaveFormat.Html);
            return tempFile;
        }
    }
}
```

### Voir aussi

* class [HtmlConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Convertit le fichier entre le html et d'autres formats de fichiers de feuille de calcul.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Options d'entrée et de chargement |
| saveOptions | LowCodeSaveOptions | Options de sortie et d'enregistrement |

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class HtmlConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // Créer un modèle HTML simple en mémoire
            string htmlContent = "<html><body><h1>Test Document</h1><p>This is a test HTML document.</p></body></html>";
            using (MemoryStream template = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(htmlContent)))
            {
                // Convertir en PDF en utilisant les options LowCode
                HtmlConverter.Process(
                    new LowCodeLoadOptions() { InputStream = template },
                    new LowCodeSaveOptions()
                    {
                        OutputFile = "output.pdf",
                        SaveFormat = SaveFormat.Pdf
                    });

                // Réinitialiser la position du flux pour la conversion suivante
                template.Position = 0;

                // Convertir en HTML en utilisant les options LowCode
                HtmlConverter.Process(
                    new LowCodeLoadOptions() { InputStream = template },
                    new LowCodeSaveOptions()
                    {
                        OutputFile = "output.html",
                        SaveFormat = SaveFormat.Html
                    });
            }

            Console.WriteLine("Conversions completed successfully.");
        }
    }
}
```

### Voir aussi

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [HtmlConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


