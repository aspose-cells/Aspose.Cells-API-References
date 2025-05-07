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
// Called: options.OperationType = PasteOperationType.Divide;
[Test]
        public void Type_PasteOperationType()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CellsNet48164.xlsx");
            Cells cells = wb.Worksheets[0].Cells;
            Aspose.Cells.Range s = cells.CreateRange("A2:B4");
            Aspose.Cells.Range d = cells.CreateRange("D9:E11");
            PasteOptions options = new PasteOptions();
            options.OperationType = PasteOperationType.Divide;
            d.Copy(s, options);
            Assert.AreEqual(0, d[0, 0].DoubleValue);
            Assert.AreEqual(CellValueType.IsNull, d[0, 1].Type);
            Assert.AreEqual(2.5, d[1, 0].DoubleValue);
            Assert.AreEqual(7, d[1, 1].DoubleValue);
            Assert.AreEqual("sd", d[2, 0].StringValue);
            Assert.AreEqual(true, d[2, 1].BoolValue);
            wb.Save(Constants.destPath + "CellsNet48164.xlsx");
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


