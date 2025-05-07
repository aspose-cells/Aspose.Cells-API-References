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
[Test]
        public void Type_MergedCellsShrinkType()
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

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


