---
title: Cells.GetMaxGroupedRowOutlineLevel
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets the max grouped row outline level zerobased
type: docs
url: /net/aspose.cells/cells/getmaxgroupedrowoutlinelevel/
---
## Cells.GetMaxGroupedRowOutlineLevel method

Gets the max grouped row outline level (zero-based).

```csharp
public int GetMaxGroupedRowOutlineLevel()
```

### Return Value

The max grouped row outline level (zero-based)

### Examples

```csharp
// Called: if (cellsSrc.GetMaxGroupedRowOutlineLevel() != 0)
public static void Cells_Method_GetMaxGroupedRowOutlineLevel(Worksheet sheetSrc, Worksheet sheetDest, string info)
        {      
            Cells cellsSrc = sheetSrc.Cells;
            Cells cellsDest = sheetDest.Cells;
            if (AssertHelper.checkNull(cellsSrc, cellsDest, info))
            {
                return;
            }           
            //====================compare row and column=====================//
            AssertHelper.AreEqual(cellsSrc.MinRow, cellsDest.MinRow, info + ".MinRow");
            AssertHelper.AreEqual(cellsSrc.MinColumn, cellsDest.MinColumn, info + ".MinColumn");
            AssertHelper.AreEqual(cellsSrc.MaxRow, cellsDest.MaxRow, info + ".MaxRow");
            AssertHelper.AreEqual(cellsSrc.MaxDataRow, cellsDest.MaxDataRow, info + ".MaxDataRow");
            AssertHelper.AreEqual(cellsSrc.MaxColumn, cellsDest.MaxColumn, info + ".MaxColumn");
            AssertHelper.AreEqual(cellsSrc.MaxDataColumn, cellsDest.MaxDataColumn, info + ".MaxDataColumn");     

            int minRow = cellsSrc.MinRow;
            int minColumn = cellsSrc.MinColumn;
            int maxRow = Math.Max(cellsSrc.MaxRow, cellsSrc.MaxDataRow);
            int maxColumn = Math.Max(cellsSrc.MaxColumn, cellsSrc.MaxDataColumn);

            for (int col = minColumn; col <= maxColumn; col ++)
            {
                AssertHelper.AreEqual(cellsSrc.GetColumnWidth(col), cellsDest.GetColumnWidth(col), delta, info + ".GetColumnWidth(" + col + ")");
                AssertHelper.AreEqual(cellsSrc.GetMaxGroupedColumnOutlineLevel(), cellsDest.GetMaxGroupedColumnOutlineLevel(), info + ".GetMaxGroupedColumnOutlineLevel()");
                if (cellsSrc.GetMaxGroupedColumnOutlineLevel() != 0)
                    AssertHelper.AreEqual(cellsSrc.GetGroupedColumnOutlineLevel(col), cellsDest.GetGroupedColumnOutlineLevel(col), info + "GetGroupedColumnOutlineLevel(" + col + ")");
            }
            for (int row = minRow; row < maxRow; row ++)
            {
                AssertHelper.AreEqual(cellsSrc.GetRowHeight(row), cellsDest.GetRowHeight(row), delta, info + ".GetRowHeight(" + row + ")");
                AssertHelper.AreEqual(cellsSrc.GetMaxGroupedRowOutlineLevel(), cellsDest.GetMaxGroupedRowOutlineLevel(), info + ".GetMaxGroupedRowOutlineLevel()");
                if (cellsSrc.GetMaxGroupedRowOutlineLevel() != 0)
                    AssertHelper.AreEqual(cellsSrc.GetGroupedRowOutlineLevel(row), cellsDest.GetGroupedRowOutlineLevel(row), info + ".GetGroupedRowOutlineLevel(" + row + ")");
            }
            AssertHelper.AreEqual(cellsSrc.StandardHeight, cellsDest.StandardHeight, delta, info + ".StandardHeight");
            AssertHelper.AreEqual(cellsSrc.StandardWidth, cellsDest.StandardWidth, delta, info + ".StandardWidth");
            //==============compare mergedcells===================//
            equals_MergedCells(cellsSrc, cellsDest, info);
            //==============compare range=======================//
            RangesTest.Cells_Method_GetMaxGroupedRowOutlineLevel(cellsSrc.Ranges, cellsDest.Ranges, info + ".Ranges");
            //==============compare column and row=======================//
            ColumnsTest.Cells_Method_GetMaxGroupedRowOutlineLevel(cellsSrc.Columns, cellsDest.Columns, info + ".Columns");
            RowsTest.Cells_Method_GetMaxGroupedRowOutlineLevel(cellsSrc.Rows, cellsDest.Rows, info + ".Rows");
            //===============compare cell======================//
            for (IEnumerator ie = cellsSrc.GetEnumerator(); ie.MoveNext(); )
            {
                Cell cellSrc = (Cell)ie.Current;
                int row = cellSrc.Row;
                int col = cellSrc.Column;
                Cell cellDest = cellsDest[row, col];
                CellTest.Cells_Method_GetMaxGroupedRowOutlineLevel(cellSrc, cellDest, info + "[" + row + "," + col + "]");

            }

            AssertHelper.AreEqual(cellsSrc.PreserveString, cellsDest.PreserveString, info + ".PreserveString");
            //cellsSrc.GetCellOrNull
            //cellsSrc.GetEnumerator
            //cellsSrc.GetRowEnumerator();
            //cellsSrc.GetRowOrNull
            //AssertHelper.AreEqual(cellsSrc.IsDefaultRowHeightMatched, cellsDest.IsDefaultRowHeightMatched, info + ".IsDefaultRowHeightMatched");
            //AssertHelper.AreEqual(cellsSrc.MaxGroupColumnsLevel, cellsDest.MaxGroupColumnsLevel, info + ".MaxGroupColumnsLevel");
            //AssertHelper.AreEqual(cellsSrc.MaxGroupRowsLevel, cellsDest.MaxGroupRowsLevel, info + ".MaxGroupRowsLevel");
            //AssertHelper.AreEqual(cellsSrc.GetKeepedPivotRanges();    

        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


