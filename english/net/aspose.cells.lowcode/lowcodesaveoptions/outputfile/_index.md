---
title: LowCodeSaveOptions.OutputFile
second_title: Aspose.Cells for .NET API Reference
description: LowCodeSaveOptions property. Gets and sets the filewith path if needed for saving the generated data. When setting this property with value other than null or empty string OutputStream will be ignored
type: docs
url: /net/aspose.cells.lowcode/lowcodesaveoptions/outputfile/
---
## LowCodeSaveOptions.OutputFile property

Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [`OutputStream`](../outputstream/) will be ignored.

```csharp
public string OutputFile { get; set; }
```

### Examples

```csharp
// Called: OutputFile = Constants.checkPath + "License/LowCode" + fnTail
private void LowCodeSaveOptions_Property_OutputFile(Stream template, SaveOptions saveOptions, string fnTail)
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

* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


