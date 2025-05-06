---
title: Cells.MaxColumn
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Maximum column index of those cells that have been instantiated in the collectiondoes not include the column where style is defined for the whole column but no cell has been instantiated in it
type: docs
url: /net/aspose.cells/cells/maxcolumn/
---
## Cells.MaxColumn property

Maximum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it).

```csharp
public int MaxColumn { get; }
```

### Remarks

Return -1 if there is no cell has been instantiated.

### Examples

```csharp
// Called: ca = CellArea.CreateCellArea(4, 0, cells.MaxRow, cells.MaxColumn);
[Test]
        public void Property_MaxColumn()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet40697.xls&quot;);
            Cells cells = workbook.Worksheets[0].Cells;
            CellArea ca = CellArea.CreateCellArea(4, 0, cells.MaxRow, cells.MaxColumn);

            cells.Subtotal(ca, 0, ConsolidationFunction.CountNums, new int[] { 0 }, true, false, true);
            ca = CellArea.CreateCellArea(4, 0, cells.MaxRow, cells.MaxColumn);
            cells.Subtotal(ca, 2, ConsolidationFunction.CountNums, new int[] { 2 }, false, false, true);

            Assert.AreEqual(cells[&quot;B140&quot;].StringValue, &quot;WINSALEM  Count&quot;);
            Assert.AreEqual(cells[&quot;A141&quot;].StringValue, &quot;NC Count&quot;);
            Assert.AreEqual(cells[&quot;B142&quot;].StringValue, &quot;Grand Count&quot;);
            Assert.AreEqual(cells[&quot;A143&quot;].StringValue, &quot;Grand Count&quot;);
            workbook.Save(Constants.destPath + &quot;CellsNet40697.xls&quot;);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


