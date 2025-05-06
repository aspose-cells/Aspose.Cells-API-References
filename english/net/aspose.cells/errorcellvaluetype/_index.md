---
title: Enum ErrorCellValueType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ErrorCellValueType enum. Represents a cell value which contains an error
type: docs
url: /net/aspose.cells/errorcellvaluetype/
---
## ErrorCellValueType enumeration

Represents a cell value which contains an error.

```csharp
public enum ErrorCellValueType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Blocked | `10` | Represents the value of a cell containing a #BLOCKED! error. |
| Busy | `14` | Represents the value of a cell containing a #BUSY! error. |
| Calc | `13` | Represents the value of a cell containing a #CALC! error. |
| Connect | `9` | Represents the value of a cell containing a #CONNECT! error. |
| Name | `4` | Represents the value of a cell containing a #NAME? error. |
| Field | `12` | Represents the value of a cell containing a #FIELD! error. |
| Spill | `8` | Represents the value of a cell containing a #SPILL! error. |
| Unknown | `11` | Represents the value of a cell containing a #UNKNOWN! error. |
| TimeOut | `19` | Represents the value of a cell containing a #TIMEOUT! error. |
| External | `18` | Represents the value of a cell containing an #EXTERNAL! error. |

### Examples

```csharp
// Called: Assert.AreEqual(ErrorCellValueType.Spill, c.ErrorValue);
[Test]
        public void Type_ErrorCellValueType()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET57143.xlsx&quot;);
            Workbook w = new Workbook();
            w.Worksheets[0].Copy(wb.Worksheets[0]);
            CellRichValue c = w.Worksheets[0].Cells[&quot;A1&quot;].GetRichValue();
            Assert.AreEqual(ErrorCellValueType.Spill, c.ErrorValue);
            w.Save(Constants.destPath + &quot;CELLSNET57143.xlsx&quot;);
            w = new Workbook(Constants.destPath + &quot;CELLSNET57143.xlsx&quot;);
            c = w.Worksheets[0].Cells[&quot;A1&quot;].GetRichValue();
            Assert.AreEqual(ErrorCellValueType.Spill, c.ErrorValue);
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


