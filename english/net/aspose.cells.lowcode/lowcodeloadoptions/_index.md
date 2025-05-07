---
title: Class LowCodeLoadOptions
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.LowCode.LowCodeLoadOptions class. Options for loading template file
type: docs
url: /net/aspose.cells.lowcode/lowcodeloadoptions/
---
## LowCodeLoadOptions class

Options for loading template file.

```csharp
public class LowCodeLoadOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [LowCodeLoadOptions](lowcodeloadoptions/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [InputFile](../../aspose.cells.lowcode/lowcodeloadoptions/inputfile/) { get; set; } | Gets and sets the file(with path if needed) of the template. |
| [InputStream](../../aspose.cells.lowcode/lowcodeloadoptions/inputstream/) { get; set; } | Gets and sets the Stream of the template. |

### Examples

```csharp
// Called: SpreadsheetLocker.Process(new LowCodeLoadOptions() { InputStream = stream },
private void Type_LowCodeLoadOptions(Stream stream, string fnTail)
        {
            SpreadsheetLocker.Process(new LowCodeLoadOptions() { InputStream = stream },
                new LowCodeSaveOptions()
                {
                    OutputFile = Constants.checkPath + "License/LowCodeLock" + fnTail,
                }, "123456", "234567");
        }
```

### See Also

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


