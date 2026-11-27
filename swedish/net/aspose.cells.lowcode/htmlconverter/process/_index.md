---
title: "HtmlConverter.Process"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlConverter-metod. Konverterar given mallfil mellan html och andra format"
type: docs
url: /sv/net/aspose.cells.lowcode/htmlconverter/process/
---
## Process(string, string) {#process_1}

Konverterar given mallfil mellan html och andra format.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| templateFile | String | Mallfilen som ska konverteras |
| resultFile | String | Den resulterande filen |

### Exempel

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
            // Skapa en tillfällig HTML-fil för konvertering
            string templateFile = CreateSampleHtmlFile();
            string resultFile = "HtmlConversionResult.xlsx";

            try
            {
                // Bearbeta filerna direkt med HtmlConverter
                HtmlConverter.Process(templateFile, resultFile);

                Console.WriteLine($"Successfully converted '{templateFile}' to '{resultFile}'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
            finally
            {
                // Rensa upp temporär fil
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

### Se även

* class [HtmlConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Konverterar fil mellan html och andra kalkylbladsformat.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Alternativ för indata och laddning. |
| saveOptions | LowCodeSaveOptions | Alternativ för utdata och sparning. |

### Exempel

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
            // Skapa en enkel HTML-mall i minnet
            string htmlContent = "<html><body><h1>Test Document</h1><p>This is a test HTML document.</p></body></html>";
            using (MemoryStream template = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(htmlContent)))
            {
                // Konvertera till PDF med LowCode-alternativ
                HtmlConverter.Process(
                    new LowCodeLoadOptions() { InputStream = template },
                    new LowCodeSaveOptions()
                    {
                        OutputFile = "output.pdf",
                        SaveFormat = SaveFormat.Pdf
                    });

                // Återställ strömmens position för nästa konvertering
                template.Position = 0;

                // Konvertera till HTML med LowCode-alternativ
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

### Se även

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [HtmlConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


