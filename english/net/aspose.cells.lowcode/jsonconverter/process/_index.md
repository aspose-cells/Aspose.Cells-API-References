---
title: JsonConverter.Process
second_title: Aspose.Cells for .NET API Reference
description: JsonConverter method. Converts given template file between json and other formats
type: docs
url: /net/aspose.cells.lowcode/jsonconverter/process/
---
## Process(string, string) {#process_1}

Converts given template file between json and other formats.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parameter | Type | Description |
| --- | --- | --- |
| templateFile | String | The template file to be converted |
| resultFile | String | The resultant file |

### Examples

```csharp
namespace AsposeCellsExamples.JsonConverterMethodProcessWithStringStringDemo
{
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class JsonConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // Create sample JSON data and write to temporary file
            string jsonData = "{\"employees\":[{\"name\":\"John\", \"department\":\"Sales\"}, {\"name\":\"Jane\", \"department\":\"Marketing\"}]}";
            string templatePath = "template.json";
            File.WriteAllText(templatePath, jsonData);

            string resultPath = "output.xlsx";

            try
            {
                // Process files directly using JsonConverter's static method
                JsonConverter.Process(templatePath, resultPath);

                Console.WriteLine($"Successfully converted JSON to spreadsheet. Output: {resultPath}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Conversion error: {ex.Message}");
            }
            finally
            {
                // Clean up temporary JSON file
                if (File.Exists(templatePath))
                {
                    File.Delete(templatePath);
                }
            }
        }
    }
}
```

### See Also

* class [JsonConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Converts between json data and other spreadsheet file formats.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Options for input and loading |
| saveOptions | LowCodeSaveOptions | Options for output and saving |

### Examples

```csharp
// Called: JsonConverter.Process(new LowCodeLoadOptions() { InputStream = template },
private void JsonConverter_Method_Process(Stream template, SaveOptions saveOptions, string fnTail)
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
* class [JsonConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


