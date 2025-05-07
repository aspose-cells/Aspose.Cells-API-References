---
title: Class LowCodePdfSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.LowCode.LowCodePdfSaveOptions class. Options for saving pdf in low code way
type: docs
url: /net/aspose.cells.lowcode/lowcodepdfsaveoptions/
---
## LowCodePdfSaveOptions class

Options for saving pdf in low code way.

```csharp
public class LowCodePdfSaveOptions : LowCodeSaveOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [LowCodePdfSaveOptions](lowcodepdfsaveoptions/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [`OutputStream`](../lowcodesaveoptions/outputstream/) will be ignored.(Inherited from [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Gets and sets the Stream for writing the generated data to. When setting this property with value other than null, [`OutputFile`](../lowcodesaveoptions/outputfile/) will be ignored.(Inherited from [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [PdfOptions](../../aspose.cells.lowcode/lowcodepdfsaveoptions/pdfoptions/) { get; set; } | The options for saving Pdf file. |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodepdfsaveoptions/saveformat/) { get; set; } | The save format for the output. For converting to pdf, it can only be Pdf. |

### Examples

```csharp
// Called: new LowCodePdfSaveOptions() {
private void Type_LowCodePdfSaveOptions(Stream template, SaveOptions saveOptions, string fnTail)
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

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


