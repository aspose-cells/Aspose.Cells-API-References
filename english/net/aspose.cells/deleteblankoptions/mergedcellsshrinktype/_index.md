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
// Called: dopts.MergedCellsShrinkType = MergedCellsShrinkType.KeepHeaderOnly;
[Test]
        public void Property_MergedCellsShrinkType()
        {
            Workbook wb = new Workbook();
            Style s = wb.DefaultStyle;
            s.Font.Name = "Arial";
            s.Font.Size = 10;
            wb.DefaultStyle = s;
            Cells cells = wb.Worksheets[0].Cells;

            CELLSNET56128InitCol(cells);
            cells.DeleteBlankColumns();
            AssertHelper.AssertNonEmptyCell(cells, 0, 0, "WithouOption-A1");
            AssertHelper.AssertNonEmptyCell(cells, 0, 1, "WithouOption-B1");
            AssertHelper.AssertEmptyCell(cells, 0, 2, "WithouOption-C1");

            cells.Clear();
            cells.UnMerge(0, 0, 10, 1);
            CELLSNET56128InitCol(cells);
            DeleteBlankOptions dopts = new DeleteBlankOptions();
            dopts.MergedCellsShrinkType = MergedCellsShrinkType.KeepHeaderOnly;
            cells.DeleteBlankColumns(dopts);
            AssertHelper.AssertNonEmptyCell(cells, 0, 0, "ShrinkHeader-A1");
            AssertHelper.AssertNonEmptyCell(cells, 0, 1, "ShrinkHeader-B1");
            AssertHelper.AssertEmptyCell(cells, 0, 2, "ShrinkHeader-C1");

            cells.Clear();
            cells.UnMerge(0, 0, 10, 1);
            CELLSNET56128InitCol(cells);
            dopts.MergedCellsShrinkType = MergedCellsShrinkType.None;
            cells.DeleteBlankColumns(dopts);
            AssertHelper.AssertNonEmptyCell(cells, 0, 0, "ShrinkNone-A1");
            AssertHelper.AssertEmptyCell(cells, 0, 1, "ShrinkNone-B1");
            AssertHelper.AssertEmptyCell(cells, 0, 2, "ShrinkNone-C1");
            AssertHelper.AssertNonEmptyCell(cells, 0, 3, "ShrinkNone-D1");

            cells.Clear();
            cells.UnMerge(0, 0, 10, 1);
            CELLSNET56128InitCol(cells);
            dopts.MergedCellsShrinkType = MergedCellsShrinkType.ShrinkToFit;
            cells.DeleteBlankColumns(dopts);
            AssertHelper.AssertNonEmptyCell(cells, 0, 0, "ShrinkFit-A1");
            AssertHelper.AssertEmptyCell(cells, 0, 1, "ShrinkFit-B1");
            AssertHelper.AssertNonEmptyCell(cells, 0, 2, "ShrinkFit-C1");
            AssertHelper.AssertEmptyCell(cells, 0, 3, "ShrinkFit-D1");
        }
```

### See Also

* enum [MergedCellsShrinkType](../../mergedcellsshrinktype/)
* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


