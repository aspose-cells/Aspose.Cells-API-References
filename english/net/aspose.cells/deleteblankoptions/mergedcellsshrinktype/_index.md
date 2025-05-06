---
title: DeleteBlankOptions.MergedCellsShrinkType
second_title: Aspose.Cells for .NET API Reference
description: DeleteBlankOptions property. Indicates how to process merged cells when deleting blank rows/columns
type: docs
url: /net/aspose.cells/deleteblankoptions/mergedcellsshrinktype/
---
## DeleteBlankOptions.MergedCellsShrinkType property

Indicates how to process merged cells when deleting blank rows/columns.

```csharp
public MergedCellsShrinkType MergedCellsShrinkType { get; set; }
```

### Remarks

For KeepHeaderOnly, all cells in it will be taken as blank except the non-blank top-left cell. It is the default value of this property. For None, all cells in it will be taken as non-blank. For ShrinkToFit, all cells outside the content display area will be taken as blank.

### Examples

```csharp
// Called: dbo.MergedCellsShrinkType = MergedCellsShrinkType.None;
[Test]
        public void Property_MergedCellsShrinkType()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            Cell cell = cells[2, 0];
            cells[0, 1].PutValue(1);
            cells.Merge(0, 1, 2, 2);
            cells.DeleteBlankRows();
            Assert.AreEqual(1, cells.GetMergedAreas().Length, &quot;No options, MergedAreas.Count&quot;);
            AssertHelper.checkCellArea(CellArea.CreateCellArea(0, 1, 0, 2),
                cells.GetMergedAreas()[0], &quot;No options, MergedArea&quot;);

            cell = cells[2, 0];
            cells.Merge(0, 1, 2, 2, true, true);
            DeleteBlankOptions dbo = new DeleteBlankOptions();
            cells.DeleteBlankRows(dbo); //CELLSNET-56864
            Assert.AreEqual(1, cells.GetMergedAreas().Length, &quot;Options with default shrink type, MergedAreas.Count&quot;);
            AssertHelper.checkCellArea(CellArea.CreateCellArea(0, 1, 0, 2),
                cells.GetMergedAreas()[0], &quot;Options with default shrink type, MergedArea&quot;);

            cell = cells[2, 0];
            cells.Merge(0, 1, 2, 2, true, true);
            dbo.MergedCellsShrinkType = MergedCellsShrinkType.None;
            cells.DeleteBlankRows(dbo);
            Assert.AreEqual(1, cells.GetMergedAreas().Length, &quot;Options with shrink type None, MergedAreas.Count&quot;);
            AssertHelper.checkCellArea(CellArea.CreateCellArea(0, 1, 1, 2),
                cells.GetMergedAreas()[0], &quot;Options with shrink type None, MergedArea&quot;);

            cell = cells[2, 0];
            cells.Merge(0, 1, 2, 2, true, true);
            dbo.MergedCellsShrinkType = MergedCellsShrinkType.ShrinkToFit;
            cells.DeleteBlankRows(dbo);
            Assert.AreEqual(1, cells.GetMergedAreas().Length, &quot;Options with ShrinkToFit, MergedAreas.Count&quot;);
            AssertHelper.checkCellArea(CellArea.CreateCellArea(0, 1, 0, 2),
                cells.GetMergedAreas()[0], &quot;Options with ShrinkToFit, MergedArea&quot;);
        }
```

### See Also

* enum [MergedCellsShrinkType](../../mergedcellsshrinktype/)
* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


