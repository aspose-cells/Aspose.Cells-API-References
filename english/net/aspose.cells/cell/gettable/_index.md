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
// Called: Assert.IsNotNull(cells[&amp;quot;B3&amp;quot;].GetTable());
[Test]
        public void Method_GetTable()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellTest01.xlsx&quot;);
            Cells cells = workbook.Worksheets[0].Cells;

            Assert.IsNotNull(cells[&quot;B3&quot;].GetTable());
            Assert.IsTrue(cells[&quot;F2&quot;].IsArrayFormula);
            Assert.IsTrue(cells[&quot;H3&quot;].IsSharedFormula);
            Style style = cells[&quot;F5&quot;].GetStyle();
            Assert.AreEqual(style.Borders.DiagonalStyle, CellBorderType.Thin);
           AssertHelper.AreEqual(style.Borders.DiagonalColor, Color.Red);
        }
```

### See Also

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


