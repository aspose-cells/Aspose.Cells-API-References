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
// Called: dopts.MergedCellsShrinkType = MergedCellsShrinkType.ShrinkToFit;
[Test]
        public void Type_MergedCellsShrinkType()
        {
            Workbook wb = new Workbook();
            Style s = wb.DefaultStyle;
            s.Font.Name = &quot;Arial&quot;;
            s.Font.Size = 10;
            wb.DefaultStyle = s;
            Cells cells = wb.Worksheets[0].Cells;

            CELLSNET56128InitCol(cells);
            cells.DeleteBlankColumns();
            AssertHelper.AssertNonEmptyCell(cells, 0, 0, &quot;WithouOption-A1&quot;);
            AssertHelper.AssertNonEmptyCell(cells, 0, 1, &quot;WithouOption-B1&quot;);
            AssertHelper.AssertEmptyCell(cells, 0, 2, &quot;WithouOption-C1&quot;);

            cells.Clear();
            cells.UnMerge(0, 0, 10, 1);
            CELLSNET56128InitCol(cells);
            DeleteBlankOptions dopts = new DeleteBlankOptions();
            dopts.MergedCellsShrinkType = MergedCellsShrinkType.KeepHeaderOnly;
            cells.DeleteBlankColumns(dopts);
            AssertHelper.AssertNonEmptyCell(cells, 0, 0, &quot;ShrinkHeader-A1&quot;);
            AssertHelper.AssertNonEmptyCell(cells, 0, 1, &quot;ShrinkHeader-B1&quot;);
            AssertHelper.AssertEmptyCell(cells, 0, 2, &quot;ShrinkHeader-C1&quot;);

            cells.Clear();
            cells.UnMerge(0, 0, 10, 1);
            CELLSNET56128InitCol(cells);
            dopts.MergedCellsShrinkType = MergedCellsShrinkType.None;
            cells.DeleteBlankColumns(dopts);
            AssertHelper.AssertNonEmptyCell(cells, 0, 0, &quot;ShrinkNone-A1&quot;);
            AssertHelper.AssertEmptyCell(cells, 0, 1, &quot;ShrinkNone-B1&quot;);
            AssertHelper.AssertEmptyCell(cells, 0, 2, &quot;ShrinkNone-C1&quot;);
            AssertHelper.AssertNonEmptyCell(cells, 0, 3, &quot;ShrinkNone-D1&quot;);

            cells.Clear();
            cells.UnMerge(0, 0, 10, 1);
            CELLSNET56128InitCol(cells);
            dopts.MergedCellsShrinkType = MergedCellsShrinkType.ShrinkToFit;
            cells.DeleteBlankColumns(dopts);
            AssertHelper.AssertNonEmptyCell(cells, 0, 0, &quot;ShrinkFit-A1&quot;);
            AssertHelper.AssertEmptyCell(cells, 0, 1, &quot;ShrinkFit-B1&quot;);
            AssertHelper.AssertNonEmptyCell(cells, 0, 2, &quot;ShrinkFit-C1&quot;);
            AssertHelper.AssertEmptyCell(cells, 0, 3, &quot;ShrinkFit-D1&quot;);
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


