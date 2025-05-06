---
title: PasteOptions.PasteType
second_title: Aspose.Cells for .NET API Reference
description: PasteOptions property. The paste special type
type: docs
url: /net/aspose.cells/pasteoptions/pastetype/
---
## PasteOptions.PasteType property

The paste special type.

```csharp
public PasteType PasteType { get; set; }
```

### Examples

```csharp
// Called: pos.PasteType = PasteType.ColumnWidths; // For some reason, we must first copy the column widths...
private void Property_PasteType(DataTable tbl, RepeatRange repeatRange)
        {
            if (tbl.Rows.Count == 0)
            {
                // Nothing to do
                return;
            }

            int maxNumRows = GetMaxNumRows(wbd.Workbook);
            int maxNumCols = GetMaxNumCols(wbd.Workbook);

            Aspose.Cells.Range range = GetRange(wbd.Workbook, repeatRange.RangeName, true);
            Cells cells = range.Worksheet.Cells;

            bool entireCols = range.RowCount == maxNumRows;     // If the range contains all the rows, then we should handle entire columns, not only part of them. (This is not a typo, think again if you think so)
            bool entireRows = range.ColumnCount == maxNumCols;  // If the range contains all the cols, then we should handle entire rows, not only part of them. (This is not a typo, think again if you think so)

            if (entireCols &amp;&amp; repeatRange.RepeatDirection != RangeRepeatDirection.Horizontal)
            {
                throw new ApplicationException(string.Format(&quot;The range {0} contains entire column/columns. In this case, the repeat direction must be Horizontal.&quot;, range.Name));
            }

            if (entireRows &amp;&amp; repeatRange.RepeatDirection != RangeRepeatDirection.Vertical)
            {
                throw new ApplicationException(string.Format(&quot;The range {0} contains entire row/rows. In this case, the repeat direction must be Vertical.&quot;, range.Name));
            }

            List&lt;Double&gt; columnWidths = new List&lt;double&gt;();

            if (repeatRange.RepeatDirection == RangeRepeatDirection.Horizontal)
            {
                // We need to remember all column widths to the right of the range, since inserting ranges reset the columns widths to the right
                for (int columnIndex = range.FirstColumn + range.ColumnCount; columnIndex &lt;= cells.MaxDataColumn; columnIndex++)
                {
                    Aspose.Cells.Column column = cells.Columns[columnIndex];
                    columnWidths.Add(column.Width);
                }
            }

            ShiftType shiftType = repeatRange.RepeatDirection == RangeRepeatDirection.Vertical ? ShiftType.Down : ShiftType.Right;
            int rowOffset = repeatRange.RepeatDirection == RangeRepeatDirection.Vertical ? range.RowCount : 0;
            int columnOffset = repeatRange.RepeatDirection == RangeRepeatDirection.Horizontal ? range.ColumnCount : 0;
            int insertRangeRows = repeatRange.RepeatDirection == RangeRepeatDirection.Vertical ? range.RowCount * (tbl.Rows.Count - 1) : range.RowCount;
            int insertRangeColumns = repeatRange.RepeatDirection == RangeRepeatDirection.Horizontal ? range.ColumnCount * (tbl.Rows.Count - 1) : range.ColumnCount;


            InsertRangeEx(cells, range.FirstRow + rowOffset, range.FirstColumn + columnOffset, shiftType, insertRangeRows, insertRangeColumns, entireRows, entireCols);

            for (int rowIndex = 0; rowIndex &lt; tbl.Rows.Count; rowIndex++)
            {
                DataRow row = tbl.Rows[rowIndex];
                Aspose.Cells.Range newRange = cells.CreateRange(range.FirstRow + rowOffset, range.FirstColumn + columnOffset, range.RowCount, range.ColumnCount);

                if (rowIndex &lt; tbl.Rows.Count - 1)
                {

                    if (entireCols) // Are we copying entire columns horizontally? -&gt; Use CopyColumns (this will include grouping)
                    {
                        cells.CopyColumns(cells, range.FirstColumn, range.FirstColumn + columnOffset, columnOffset);
                    }
                    else
                        if (entireRows) // Are we copying entire rows vertically? -&gt; Use CopyRows (this will include grouping)
                    {
                        cells.CopyRows(cells, range.FirstRow, range.FirstRow + rowOffset, rowOffset);
                    }
                    else // Not copying entire rows or columns, use Range.Copy instead
                    {
                        PasteOptions pos = new PasteOptions();
                        pos.PasteType = PasteType.ColumnWidths; // For some reason, we must first copy the column widths...
                        newRange.Copy(range, pos);
                        newRange.Copy(range);                   // ...and then the actual values
                    }
                }

                ReplaceTags(cells, range, row);
                range = newRange;
            }

            if (repeatRange.RepeatDirection == RangeRepeatDirection.Horizontal)
            {
                // Reset the widths of the columns to the right
                for (int i = 0; i &lt; columnWidths.Count; i++)
                {
                    Aspose.Cells.Column column = cells.Columns[i + range.FirstColumn];
                    column.Width = columnWidths[i];
                }
            }
        }
```

### See Also

* enum [PasteType](../../pastetype/)
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


