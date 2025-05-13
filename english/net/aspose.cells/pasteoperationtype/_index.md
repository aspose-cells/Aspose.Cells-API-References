---
title: Enum PasteOperationType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.PasteOperationType enum. Represents operation type when pasting range
type: docs
url: /net/aspose.cells/pasteoperationtype/
---
## PasteOperationType enumeration

Represents operation type when pasting range.

```csharp
public enum PasteOperationType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No operation. |
| Add | `1` | Add |
| Subtract | `2` | Subtract |
| Multiply | `3` | Multiply |
| Divide | `4` | Divide |

### Examples

```csharp
// Called: OperationType = PasteOperationType.None,
public void Cells_Type_PasteOperationType()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet sheet = workbook.Worksheets["test"];

    var pasteOptions = new PasteOptions()
    {
        PasteType = PasteType.Values,
        OperationType = PasteOperationType.None,
        SkipBlanks = false,
        Transpose = false
    };
    Aspose.Cells.Range range = sheet.Cells.CreateRange("A1", "E26");
    range.Copy(range, pasteOptions);
    Util.ReSave(workbook, SaveFormat.Xlsx);
    //workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


