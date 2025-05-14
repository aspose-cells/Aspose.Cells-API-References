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
public void CellRichValue_Property_ErrorValue()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Workbook w = new Workbook();
    w.Worksheets[0].Copy(wb.Worksheets[0]);
    CellRichValue c = w.Worksheets[0].Cells["A1"].GetRichValue();
    Assert.AreEqual(ErrorCellValueType.Spill, c.ErrorValue);
    w.Save(Constants.destPath + "example.xlsx");
    w = new Workbook(Constants.destPath + "example.xlsx");
    c = w.Worksheets[0].Cells["A1"].GetRichValue();
    Assert.AreEqual(ErrorCellValueType.Spill, c.ErrorValue);
}
```

### See Also

* enum [ErrorCellValueType](../../errorcellvaluetype/)
* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


