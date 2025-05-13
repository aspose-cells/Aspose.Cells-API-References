---
title: Enum MergedCellsShrinkType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.MergedCellsShrinkType enum. Represents the strategy to shrink merged cells for operations such as deleting blank rows/column
type: docs
url: /net/aspose.cells/mergedcellsshrinktype/
---
## MergedCellsShrinkType enumeration

Represents the strategy to shrink merged cells for operations such as deleting blank rows/column.

```csharp
public enum MergedCellsShrinkType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | Leaves the merged cells as it is without any modification. |
| ShrinkToFit | `1` | Shrinks the merged area if needed, by removing rows from the bottom or columns from the right, while ensuring all content remains visible. |
| KeepHeaderOnly | `2` | Only keeps the header rows/columns of the merged area when the top-left cell of the merged area is not blank. |

### Examples

```csharp
// Called: dopts.MergedCellsShrinkType = MergedCellsShrinkType.None;
public void Cells_Type_MergedCellsShrinkType()
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

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


