---
title: Cell.GetRichValue
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Gets rich value of the cell
type: docs
url: /net/aspose.cells/cell/getrichvalue/
---
## Cell.GetRichValue method

Gets rich value of the cell.

```csharp
public CellRichValue GetRichValue()
```

### Examples

```csharp
// Called: CellRichValue c = w.Worksheets[0].Cells["A1"].GetRichValue();
public void Cell_Method_GetRichValue()
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

* class [CellRichValue](../../cellrichvalue/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


