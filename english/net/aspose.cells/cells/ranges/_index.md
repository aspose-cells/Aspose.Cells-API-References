---
title: Cells.Ranges
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets the collection of Range objects created at run time
type: docs
url: /net/aspose.cells/cells/ranges/
---
## Cells.Ranges property

Gets the collection of [`Range`](../../range/) objects created at run time.

```csharp
public RangeCollection Ranges { get; }
```

### Examples

```csharp
// Called: RangesTest.equals(cellsSrc.Ranges, cellsDest.Ranges, info + ".Ranges");
public static void Property_Ranges(Worksheet sheetSrc, Worksheet sheetDest, string info)
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
            RangesTest.Property_Ranges(cellsSrc.Ranges, cellsDest.Ranges, info + ".Ranges");
            //==============compare column and row=======================//
            ColumnsTest.Property_Ranges(cellsSrc.Columns, cellsDest.Columns, info + ".Columns");
            RowsTest.Property_Ranges(cellsSrc.Rows, cellsDest.Rows, info + ".Rows");
            //===============compare cell======================//
            for (IEnumerator ie = cellsSrc.GetEnumerator(); ie.MoveNext(); )
            {
                Cell cellSrc = (Cell)ie.Current;
                int row = cellSrc.Row;
                int col = cellSrc.Column;
                Cell cellDest = cellsDest[row, col];
                CellTest.Property_Ranges(cellSrc, cellDest, info + "[" + row + "," + col + "]");

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

* class [RangeCollection](../../rangecollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


