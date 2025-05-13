---
title: Cell.GetTable
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Gets the table which contains this cell
type: docs
url: /net/aspose.cells/cell/gettable/
---
## Cell.GetTable method

Gets the table which contains this cell.

```csharp
public ListObject GetTable()
```

### Examples

```csharp
// Called: Assert.IsNotNull(cells["B3"].GetTable());
public void Cell_Method_GetTable()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Cells cells = workbook.Worksheets[0].Cells;

    Assert.IsNotNull(cells["B3"].GetTable());
    Assert.IsTrue(cells["F2"].IsArrayFormula);
    Assert.IsTrue(cells["H3"].IsSharedFormula);
    Style style = cells["F5"].GetStyle();
    Assert.AreEqual(style.Borders.DiagonalStyle, CellBorderType.Thin);
   AssertHelper.AreEqual(style.Borders.DiagonalColor, Color.Red);
}
```

### See Also

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


