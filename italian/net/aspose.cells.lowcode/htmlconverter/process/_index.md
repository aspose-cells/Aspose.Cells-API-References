---
title: "HtmlConverter.Process"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo HtmlConverter. Converte il file modello fornito tra html e altri formati"
type: docs
url: /it/net/aspose.cells.lowcode/htmlconverter/process/
---
## Process(string, string) {#process_1}

Converte il file modello fornito tra html e altri formati.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| templateFile | String | Il file modello da convertire |
| resultFile | String | Il file risultante |

### Esempi

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
            // Crea un file HTML temporaneo per la conversione
            string templateFile = CreateSampleHtmlFile();
            string resultFile = "HtmlConversionResult.xlsx";

            try
            {
                // Elabora i file direttamente usando HtmlConverter
                HtmlConverter.Process(templateFile, resultFile);

                Console.WriteLine($"Successfully converted '{templateFile}' to '{resultFile}'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
            finally
            {
                // Rimuovi il file temporaneo
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

### Vedi anche

* class [HtmlConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Converte il file tra html e altri formati di file di foglio di calcolo.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Opzioni per l'input e il caricamento |
| saveOptions | LowCodeSaveOptions | Opzioni per l'output e il salvataggio |

### Esempi

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
            // Crea un semplice modello HTML in memoria
            string htmlContent = "<html><body><h1>Test Document</h1><p>This is a test HTML document.</p></body></html>";
            using (MemoryStream template = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(htmlContent)))
            {
                // Converti in PDF usando le opzioni LowCode
                HtmlConverter.Process(
                    new LowCodeLoadOptions() { InputStream = template },
                    new LowCodeSaveOptions()
                    {
                        OutputFile = "output.pdf",
                        SaveFormat = SaveFormat.Pdf
                    });

                // Reimposta la posizione dello stream per la conversione successiva
                template.Position = 0;

                // Converti in HTML usando le opzioni LowCode
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

### Vedi anche

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [HtmlConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


