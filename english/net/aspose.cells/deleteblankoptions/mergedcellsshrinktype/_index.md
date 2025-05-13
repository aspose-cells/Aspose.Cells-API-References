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
// Called: dopts.MergedCellsShrinkType = MergedCellsShrinkType.ShrinkToFit;
public void DeleteBlankOptions_Property_MergedCellsShrinkType()
{
    Workbook wb = new Workbook();
    Style s = wb.DefaultStyle;
    s.Font.Name = "Arial";
    s.Font.Size = 10;
    wb.DefaultStyle = s;
    Cells cells = wb.Worksheets[0].Cells;
    cells.SetColumnWidthPixel(0, 150);

    CELLSNET56128InitRow(cells);
    cells.DeleteBlankRows();
    AssertHelper.AssertNonEmptyCell(cells, 0, 0, "WithouOption-A1");
    AssertHelper.AssertNonEmptyCell(cells, 1, 0, "WithouOption-A2");
    AssertHelper.AssertEmptyCell(cells, 2, 0, "WithouOption-A3");

    cells.Clear();
    cells.UnMerge(0, 0, 10, 1);
    CELLSNET56128InitRow(cells);
    DeleteBlankOptions dopts = new DeleteBlankOptions();
    dopts.MergedCellsShrinkType = MergedCellsShrinkType.KeepHeaderOnly;
    cells.DeleteBlankRows(dopts);
    AssertHelper.AssertNonEmptyCell(cells, 0, 0, "ShrinkHeader-A1");
    AssertHelper.AssertNonEmptyCell(cells, 1, 0, "ShrinkHeader-A2");
    AssertHelper.AssertEmptyCell(cells, 2, 0, "ShrinkHeader-A3");

    cells.Clear();
    cells.UnMerge(0, 0, 10, 1);
    CELLSNET56128InitRow(cells);
    dopts.MergedCellsShrinkType = MergedCellsShrinkType.None;
    cells.DeleteBlankRows(dopts);
    AssertHelper.AssertNonEmptyCell(cells, 0, 0, "ShrinkNone-A1");
    AssertHelper.AssertEmptyCell(cells, 1, 0, "ShrinkNone-A2");
    AssertHelper.AssertEmptyCell(cells, 2, 0, "ShrinkNone-A3");
    AssertHelper.AssertNonEmptyCell(cells, 3, 0, "ShrinkNone-A4");

    cells.Clear();
    cells.UnMerge(0, 0, 10, 1);
    CELLSNET56128InitRow(cells);
    dopts.MergedCellsShrinkType = MergedCellsShrinkType.ShrinkToFit;
    cells.DeleteBlankRows(dopts);
    AssertHelper.AssertNonEmptyCell(cells, 0, 0, "ShrinkFit-A1");
    AssertHelper.AssertEmptyCell(cells, 1, 0, "ShrinkFit-A2");
    AssertHelper.AssertNonEmptyCell(cells, 2, 0, "ShrinkFit-A3");
    AssertHelper.AssertEmptyCell(cells, 3, 0, "ShrinkFit-A4");
}
```

### See Also

* enum [MergedCellsShrinkType](../../mergedcellsshrinktype/)
* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


