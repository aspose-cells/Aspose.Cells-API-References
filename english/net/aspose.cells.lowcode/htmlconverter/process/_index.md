---
title: HtmlConverter.Process
second_title: Aspose.Cells for .NET API Reference
description: HtmlConverter method. Converts given template file between html and other formats
type: docs
url: /net/aspose.cells.lowcode/htmlconverter/process/
---
## Process(string, string) {#process_1}

Converts given template file between html and other formats.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parameter | Type | Description |
| --- | --- | --- |
| templateFile | String | The template file to be converted |
| resultFile | String | The resultant file |

### Examples

```csharp
namespace AsposeCellsExamples.HtmlConverterMethodProcessWithStringStringDemo
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class HtmlConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // Create temporary HTML file for conversion
            string templateFile = CreateSampleHtmlFile();
            string resultFile = "HtmlConversionResult.xlsx";

            try
            {
                // Process the files directly using HtmlConverter
                HtmlConverter.Process(templateFile, resultFile);

                Console.WriteLine($"Successfully converted '{templateFile}' to '{resultFile}'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
            finally
            {
                // Clean up temporary file
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

### See Also

* class [HtmlConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Converts file between html and other spreadsheet file formats.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Options for input and loading |
| saveOptions | LowCodeSaveOptions | Options for output and saving |

### Examples

```csharp
// Called: HtmlConverter.Process(new LowCodeLoadOptions() { InputStream = template },
private void HtmlConverter_Method_Process(Stream template, SaveOptions saveOptions, string fnTail)
        {
            switch (saveOptions.SaveFormat)
            {
                case SaveFormat.Pdf:
                {
                    PdfConverter.Process(new LowCodeLoadOptions() { InputStream = template },
                        new LowCodePdfSaveOptions() {
                            OutputFile = Constants.checkPath + "License/LowCode" + fnTail,
                            PdfOptions = (PdfSaveOptions)saveOptions,
                        });
                    return;
                }
                case SaveFormat.Json:
                {
                    JsonConverter.Process(new LowCodeLoadOptions() { InputStream = template },
                        new LowCodeSaveOptions()
                        {
                            OutputFile = Constants.checkPath + "License/LowCode" + fnTail
                        });
                    return;
                }
                case SaveFormat.Html:
                {
                    HtmlConverter.Process(new LowCodeLoadOptions() { InputStream = template },
                        new LowCodeSaveOptions()
                        {
                            OutputFile = Constants.checkPath + "License/LowCode" + fnTail
                        });
                    return;
                }
                case SaveFormat.Csv:
                {
                    TextConverter.Process(new LowCodeLoadOptions() { InputStream = template },
                        new LowCodeSaveOptions()
                        {
                            OutputFile = Constants.checkPath + "License/LowCode" + fnTail
                        });
                    return;
                }
                default:
                {
                    Assert.Fail("Unsupported save format for LowCode: " + saveOptions.SaveFormat);
                    return;
                }
            }
        }
```

### See Also

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [HtmlConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


