---
title: Cells.GetMaxGroupedColumnOutlineLevel
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets the max grouped column outline level zerobased
type: docs
url: /net/aspose.cells/cells/getmaxgroupedcolumnoutlinelevel/
---
## Cells.GetMaxGroupedColumnOutlineLevel method

Gets the max grouped column outline level (zero-based).

```csharp
public int GetMaxGroupedColumnOutlineLevel()
```

### Return Value

The max grouped column outline level (zero-based)

### Examples

```csharp
// Called: if (cellsSrc.GetMaxGroupedColumnOutlineLevel() != 0)
public static void Method_GetMaxGroupedColumnOutlineLevel(Worksheet sheetSrc, Worksheet sheetDest, string info)
        {      
            Cells cellsSrc = sheetSrc.Cells;
            Cells cellsDest = sheetDest.Cells;
            if (AssertHelper.checkNull(cellsSrc, cellsDest, info))
            {
                return;
            }           
            //====================compare row and column=====================//
            AssertHelper.AreEqual(cellsSrc.MinRow, cellsDest.MinRow, info + &quot;.MinRow&quot;);
            AssertHelper.AreEqual(cellsSrc.MinColumn, cellsDest.MinColumn, info + &quot;.MinColumn&quot;);
            AssertHelper.AreEqual(cellsSrc.MaxRow, cellsDest.MaxRow, info + &quot;.MaxRow&quot;);
            AssertHelper.AreEqual(cellsSrc.MaxDataRow, cellsDest.MaxDataRow, info + &quot;.MaxDataRow&quot;);
            AssertHelper.AreEqual(cellsSrc.MaxColumn, cellsDest.MaxColumn, info + &quot;.MaxColumn&quot;);
            AssertHelper.AreEqual(cellsSrc.MaxDataColumn, cellsDest.MaxDataColumn, info + &quot;.MaxDataColumn&quot;);     

            int minRow = cellsSrc.MinRow;
            int minColumn = cellsSrc.MinColumn;
            int maxRow = Math.Max(cellsSrc.MaxRow, cellsSrc.MaxDataRow);
            int maxColumn = Math.Max(cellsSrc.MaxColumn, cellsSrc.MaxDataColumn);

            for (int col = minColumn; col &lt;= maxColumn; col ++)
            {
                AssertHelper.AreEqual(cellsSrc.GetColumnWidth(col), cellsDest.GetColumnWidth(col), delta, info + &quot;.GetColumnWidth(&quot; + col + &quot;)&quot;);
                AssertHelper.AreEqual(cellsSrc.GetMaxGroupedColumnOutlineLevel(), cellsDest.GetMaxGroupedColumnOutlineLevel(), info + &quot;.GetMaxGroupedColumnOutlineLevel()&quot;);
                if (cellsSrc.GetMaxGroupedColumnOutlineLevel() != 0)
                    AssertHelper.AreEqual(cellsSrc.GetGroupedColumnOutlineLevel(col), cellsDest.GetGroupedColumnOutlineLevel(col), info + &quot;GetGroupedColumnOutlineLevel(&quot; + col + &quot;)&quot;);
            }
            for (int row = minRow; row &lt; maxRow; row ++)
            {
                AssertHelper.AreEqual(cellsSrc.GetRowHeight(row), cellsDest.GetRowHeight(row), delta, info + &quot;.GetRowHeight(&quot; + row + &quot;)&quot;);
                AssertHelper.AreEqual(cellsSrc.GetMaxGroupedRowOutlineLevel(), cellsDest.GetMaxGroupedRowOutlineLevel(), info + &quot;.GetMaxGroupedRowOutlineLevel()&quot;);
                if (cellsSrc.GetMaxGroupedRowOutlineLevel() != 0)
                    AssertHelper.AreEqual(cellsSrc.GetGroupedRowOutlineLevel(row), cellsDest.GetGroupedRowOutlineLevel(row), info + &quot;.GetGroupedRowOutlineLevel(&quot; + row + &quot;)&quot;);
            }
            AssertHelper.AreEqual(cellsSrc.StandardHeight, cellsDest.StandardHeight, delta, info + &quot;.StandardHeight&quot;);
            AssertHelper.AreEqual(cellsSrc.StandardWidth, cellsDest.StandardWidth, delta, info + &quot;.StandardWidth&quot;);
            //==============compare mergedcells===================//
            equals_MergedCells(cellsSrc, cellsDest, info);
            //==============compare range=======================//
            RangesTest.Method_GetMaxGroupedColumnOutlineLevel(cellsSrc.Ranges, cellsDest.Ranges, info + &quot;.Ranges&quot;);
            //==============compare column and row=======================//
            ColumnsTest.Method_GetMaxGroupedColumnOutlineLevel(cellsSrc.Columns, cellsDest.Columns, info + &quot;.Columns&quot;);
            RowsTest.Method_GetMaxGroupedColumnOutlineLevel(cellsSrc.Rows, cellsDest.Rows, info + &quot;.Rows&quot;);
            //===============compare cell======================//
            for (IEnumerator ie = cellsSrc.GetEnumerator(); ie.MoveNext(); )
            {
                Cell cellSrc = (Cell)ie.Current;
                int row = cellSrc.Row;
                int col = cellSrc.Column;
                Cell cellDest = cellsDest[row, col];
                CellTest.Method_GetMaxGroupedColumnOutlineLevel(cellSrc, cellDest, info + &quot;[&quot; + row + &quot;,&quot; + col + &quot;]&quot;);

            }

            AssertHelper.AreEqual(cellsSrc.PreserveString, cellsDest.PreserveString, info + &quot;.PreserveString&quot;);
            //cellsSrc.GetCellOrNull
            //cellsSrc.GetEnumerator
            //cellsSrc.GetRowEnumerator();
            //cellsSrc.GetRowOrNull
            //AssertHelper.AreEqual(cellsSrc.IsDefaultRowHeightMatched, cellsDest.IsDefaultRowHeightMatched, info + &quot;.IsDefaultRowHeightMatched&quot;);
            //AssertHelper.AreEqual(cellsSrc.MaxGroupColumnsLevel, cellsDest.MaxGroupColumnsLevel, info + &quot;.MaxGroupColumnsLevel&quot;);
            //AssertHelper.AreEqual(cellsSrc.MaxGroupRowsLevel, cellsDest.MaxGroupRowsLevel, info + &quot;.MaxGroupRowsLevel&quot;);
            //AssertHelper.AreEqual(cellsSrc.GetKeepedPivotRanges();    

        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


