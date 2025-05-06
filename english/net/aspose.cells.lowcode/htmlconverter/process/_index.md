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
private void Method_LowCodeSaveOptions_(Stream template, SaveOptions saveOptions, string fnTail)
        {
            switch (saveOptions.SaveFormat)
            {
                case SaveFormat.Pdf:
                {
                    PdfConverter.Process(new LowCodeLoadOptions() { InputStream = template },
                        new LowCodePdfSaveOptions() {
                            OutputFile = Constants.checkPath + &quot;License/LowCode&quot; + fnTail,
                            PdfOptions = (PdfSaveOptions)saveOptions,
                        });
                    return;
                }
                case SaveFormat.Json:
                {
                    JsonConverter.Process(new LowCodeLoadOptions() { InputStream = template },
                        new LowCodeSaveOptions()
                        {
                            OutputFile = Constants.checkPath + &quot;License/LowCode&quot; + fnTail
                        });
                    return;
                }
                case SaveFormat.Html:
                {
                    HtmlConverter.Process(new LowCodeLoadOptions() { InputStream = template },
                        new LowCodeSaveOptions()
                        {
                            OutputFile = Constants.checkPath + &quot;License/LowCode&quot; + fnTail
                        });
                    return;
                }
                case SaveFormat.Csv:
                {
                    TextConverter.Process(new LowCodeLoadOptions() { InputStream = template },
                        new LowCodeSaveOptions()
                        {
                            OutputFile = Constants.checkPath + &quot;License/LowCode&quot; + fnTail
                        });
                    return;
                }
                default:
                {
                    Assert.Fail(&quot;Unsupported save format for LowCode: &quot; + saveOptions.SaveFormat);
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


