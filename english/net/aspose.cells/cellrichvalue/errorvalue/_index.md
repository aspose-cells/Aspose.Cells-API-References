---
title: CellRichValue.ErrorValue
second_title: Aspose.Cells for .NET API Reference
description: CellRichValue property. Gets the error value type of the cell
type: docs
url: /net/aspose.cells/cellrichvalue/errorvalue/
---
## CellRichValue.ErrorValue property

Gets the error value type of the cell.

```csharp
public virtual ErrorCellValueType ErrorValue { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(ErrorCellValueType.Spill, c.ErrorValue);
[Test]
        public void Property_ErrorValue()
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

* enum [ErrorCellValueType](../../errorcellvaluetype/)
* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


