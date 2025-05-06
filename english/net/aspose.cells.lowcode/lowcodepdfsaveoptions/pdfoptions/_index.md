---
title: LowCodePdfSaveOptions.PdfOptions
second_title: Aspose.Cells for .NET API Reference
description: LowCodePdfSaveOptions property. The options for saving Pdf file
type: docs
url: /net/aspose.cells.lowcode/lowcodepdfsaveoptions/pdfoptions/
---
## LowCodePdfSaveOptions.PdfOptions property

The options for saving Pdf file.

```csharp
public PdfSaveOptions PdfOptions { get; set; }
```

### Examples

```csharp
// Called: PdfOptions = (PdfSaveOptions)saveOptions,
private void Property_PdfOptions(Stream template, SaveOptions saveOptions, string fnTail)
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

* class [PdfSaveOptions](../../../aspose.cells/pdfsaveoptions/)
* class [LowCodePdfSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


