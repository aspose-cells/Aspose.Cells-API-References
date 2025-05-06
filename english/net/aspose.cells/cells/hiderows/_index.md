---
title: Cells.HideRows
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Hides multiple rows
type: docs
url: /net/aspose.cells/cells/hiderows/
---
## Cells.HideRows method

Hides multiple rows.

```csharp
public void HideRows(int row, int totalRows)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| totalRows | Int32 | The row number. |

### Examples

```csharp
// Called: cells.HideRows(0, firstRow);
int Method_Int32_(Workbook wb, String rangeName)
        {
            int sheetIdx = -1; // return value
            String xlRange = rangeName;

            Name name = wb.Worksheets.Names[xlRange];

            // Set the workbook options

            Aspose.Cells.Range rng = name.GetRange();
            Worksheet sheetFromRange = rng.Worksheet;
            int origIdx = sheetFromRange.Index;

            int firstCol = rng.FirstColumn;
            int firstRow = rng.FirstRow;
            int colCnt = rng.ColumnCount;
            int rowCnt = rng.RowCount;

            // Always create a copy of the worksheet - only the copy will be modified
            sheetIdx = wb.Worksheets.AddCopy(origIdx);

            // redefine the ranges
            wb.Worksheets.ActiveSheetIndex = (sheetIdx);
            Worksheet sheet = wb.Worksheets[sheetIdx];
            Cells cells = sheet.Cells;
            rng = cells.CreateRange(firstRow, firstCol, rowCnt, colCnt);

            // process the data in the named range.

            // Determine the last used Row and Column in the *Worksheet* (i.e. not the  export range)
            int lastUsedCol = Math.Max(cells.MaxDisplayRange.ColumnCount, cells.Columns.Count);
            int lastUsedRow = Math.Max(cells.MaxDisplayRange.RowCount, cells.Rows.Count);

            // Get the last row/col of the export range
            int lastCol = firstCol + colCnt;
            int lastRow = firstRow + rowCnt;

            // It has been observed that the column widths and row heights are not &apos;pixel-perfect&apos;.
            // The following code is added to account for the deltas between the row/col sizes in Excel.
            for (int col = firstCol; col &lt; lastCol; col++)
            {
                int curWidth = cells.GetColumnWidthPixel(col);
                if (curWidth &gt; 2)
                {
                    cells.SetColumnWidthPixel(col, curWidth - 1);
                }
            }

            for (int row = firstRow; row &lt; lastRow; row++)
            {
                int curHeight = cells.GetRowHeightPixel(row);
                if (curHeight &gt; 2)
                {
                    cells.SetRowHeightPixel(row, curHeight - 1);
                }
            }

            // HIDE all the COLUMNS that are not part of the range (zero-based)
            if (firstCol &gt; 0)
            {
                cells.HideColumns(0, firstCol);
            }

            if (lastCol &lt; lastUsedCol)
            {
                // Note: the 2nd param in hideColumns is the num of cols to hide; not the ending
                // col index so add 1
                int hiddenCols = lastUsedCol + 1 - lastCol;
                cells.HideColumns(lastCol, hiddenCols);
            }

            // HIDE all the ROWS that are not part of the range (zero-based)
            if (firstRow &gt; 0)
            {
                cells.HideRows(0, firstRow);
            }

            if (lastRow &lt; lastUsedRow)
            {
                // Note: the 2nd param in hideRows is the num of rows to hide; not the ending
                // row index so add 1
                int hiddenRows = lastUsedRow + 1 - lastRow;
                cells.HideRows(lastRow, hiddenRows);

            }
            else if (colCnt == 1 &amp;&amp; rng[rowCnt - 1, 0].Type == CellValueType.IsNull)
            {
                // TODO:This circumvents Aspose Words bug &quot;WORDSNET-13180&quot; where the named range
                // has an empty cell and is outside of the &quot;used range&quot; (i.e. beyond maxRow).
                // Here, we add a dummy value to the cell underneath the last cell of the named
                // range and hide the row (so that it is not exported).
                cells[lastRow, firstCol].Value = (&quot; &quot;);
                cells.HideRow(lastRow);
            }

            // remove the background image if any - this avoids the need for a temp folder
            sheet.BackgroundImage = (null);

            return sheetIdx;
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


