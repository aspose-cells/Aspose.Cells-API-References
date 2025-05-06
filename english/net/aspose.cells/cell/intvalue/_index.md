---
title: Cell.IntValue
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets the integer value contained in the cell
type: docs
url: /net/aspose.cells/cell/intvalue/
---
## Cell.IntValue property

Gets the integer value contained in the cell.

```csharp
public int IntValue { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(i - 8, cells[i, 0].IntValue, &amp;quot;FromPartialInSub-Row-&amp;quot; + i);
[Test]
        public void Property_IntValue()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            DataSorter sorter = wb.DataSorter;
            sorter.AddKey(0, SortOrder.Descending);

            for (int i = 0; i &lt; 14; i++)
            {
                cells[i, 0].PutValue(i);
            }
            cells.GroupRows(0, 2);
            sorter.Sort(cells, 3, 0, 13, 0);
            for (int i = 0; i &lt; 14; i++)
            {
                if (i &lt; 3)
                {
                    Assert.AreEqual(1, cells.Rows[i].GroupLevel, &quot;FromEnd-Row.GroupLevel-&quot; + i);
                    Assert.AreEqual(i, cells[i, 0].IntValue, &quot;FromEnd-Row-&quot; + i);
                }
                else
                {
                    Assert.AreEqual(0, cells.Rows[i].GroupLevel, &quot;FromEnd-Row.GroupLevel-&quot; + i);
                    Assert.AreEqual(16 - i, cells[i, 0].IntValue, &quot;FromEnd-Row-&quot; + i);
                }
            }

            cells.Clear();
            for (int i = 0; i &lt; 14; i++)
            {
                cells[i, 0].PutValue(i);
            }
            cells.GroupRows(0, 2);
            sorter.Sort(cells, 2, 0, 13, 0);
            for (int i = 0; i &lt; 14; i++)
            {
                if (i &lt; 10)
                {
                    Assert.AreEqual(0, cells.Rows[i].GroupLevel, &quot;FromPartial-Row.GroupLevel-&quot; + i);
                    Assert.AreEqual(13 - i, cells[i, 0].IntValue, &quot;FromPartial-Row-&quot; + i);
                }
                else
                {
                    Assert.AreEqual(i &lt; 13 ? 1 : 0, cells.Rows[i].GroupLevel, &quot;FromPartial-Row.GroupLevel-&quot; + i);
                    Assert.AreEqual(i - 10, cells[i, 0].IntValue, &quot;FromPartial-Row-&quot; + i);
                }
            }

            //CELLSJAVA-45402: first row should not be sorted
            cells.Clear();
            for (int i = 0; i &lt; 14; i++)
            {
                cells[i, 0].PutValue(i);
            }
            cells.GroupRows(1, 2);
            sorter.Sort(cells, 2, 0, 13, 0);
            Assert.AreEqual(0, cells.Rows[0].GroupLevel, &quot;FromPartial-Row.GroupLevel-0&quot;);
            Assert.AreEqual(0, cells[0, 0].IntValue, &quot;FromPartial-Row-0&quot;);
            for (int i = 1; i &lt; 14; i++)
            {
                if (i &lt; 11)
                {
                    Assert.AreEqual(0, cells.Rows[i].GroupLevel, &quot;FromPartial-Row.GroupLevel-&quot; + i);
                    Assert.AreEqual(14 - i, cells[i, 0].IntValue, &quot;FromPartial-Row-&quot; + i);
                }
                else
                {
                    Assert.AreEqual(i &lt; 13 ? 1 : 0, cells.Rows[i].GroupLevel, &quot;FromPartial-Row.GroupLevel-&quot; + i);
                    Assert.AreEqual(i - 10, cells[i, 0].IntValue, &quot;FromPartial-Row-&quot; + i);
                }
            }

            cells.Clear();
            for (int i = 0; i &lt; 14; i++)
            {
                cells[i, 0].PutValue(i);
            }
            cells.GroupRows(0, 2);
            cells.GroupRows(0, 4);
            sorter.Sort(cells, 2, 0, 13, 0);
            for (int i = 0; i &lt; 14; i++)
            {
                if (i &lt; 8)
                {
                    Assert.AreEqual(0, cells.Rows[i].GroupLevel, &quot;FromPartialInSub-Row.GroupLevel-&quot; + i);
                    Assert.AreEqual(13 - i, cells[i, 0].IntValue, &quot;FromPartialInSub-Row-&quot; + i);
                }
                else
                {
                    Assert.AreEqual(i &lt; 11 ? 2 : (i &lt; 13 ? 1 : 0), cells.Rows[i].GroupLevel,
                        &quot;FromPartialInSub-Row.GroupLevel-&quot; + i);
                    Assert.AreEqual(i - 8, cells[i, 0].IntValue, &quot;FromPartialInSub-Row-&quot; + i);
                }
            }

            cells.Clear();
            for (int i = 0; i &lt; 14; i++)
            {
                cells[i, 0].PutValue(i);
            }
            cells.GroupRows(0, 2);
            cells.GroupRows(0, 4);
            sorter.Sort(cells, 3, 0, 13, 0);
            for (int i = 0; i &lt; 14; i++)
            {
                if (i &lt; 8)
                {
                    Assert.AreEqual(0, cells.Rows[i].GroupLevel, &quot;FromPartialAfterSub-Row.GroupLevel-&quot; + i);
                    Assert.AreEqual(13 - i, cells[i, 0].IntValue, &quot;FromPartialAfterSub-Row-&quot; + i);
                }
                else
                {
                    Assert.AreEqual(i &lt; 11 ? 2 : (i &lt; 13 ? 1 : 0), cells.Rows[i].GroupLevel,
                        &quot;FromPartialAfterSub-Row.GroupLevel-&quot; + i);
                    Assert.AreEqual(i - 8, cells[i, 0].IntValue, &quot;FromPartialAfterSub-Row-&quot; + i);
                }
            }

            cells.Clear();
            for (int i = 0; i &lt; 14; i++)
            {
                cells[i, 0].PutValue(i);
            }
            cells.GroupRows(0, 2);
            cells.GroupRows(0, 13);
            sorter.Sort(cells, 2, 0, 13, 0);
            for (int i = 0; i &lt; 14; i++)
            {
                if (i &lt; 10)
                {
                    Assert.AreEqual(1, cells.Rows[i].GroupLevel, &quot;WithinGroup-Row.GroupLevel-&quot; + i);
                    Assert.AreEqual(13 - i, cells[i, 0].IntValue, &quot;WithinGroup-Row-&quot; + i);
                }
                else
                {
                    Assert.AreEqual(i &lt; 13 ? 2 : 1, cells.Rows[i].GroupLevel, &quot;WithinGroup-Row.GroupLevel-&quot; + i);
                    Assert.AreEqual(i - 10, cells[i, 0].IntValue, &quot;WithinGroup-Row-&quot; + i);
                }
            }

            cells.Clear();
            for (int i = 0; i &lt; 14; i++)
            {
                cells[i, 0].PutValue(i);
            }
            cells.GroupRows(0, 2);
            cells.GroupRows(7, 12);
            sorter.Sort(cells, 2, 0, 13, 0);
            for (int i = 0; i &lt; 14; i++)
            {
                if (i &lt; 7)
                {
                    Assert.AreEqual(i &lt; 6 ? 1 : 0, cells.Rows[i].GroupLevel, &quot;CoverLastEnd-Row.GroupLevel-&quot; + i);
                    Assert.AreEqual(i + 7, cells[i, 0].IntValue, &quot;CoverLastEnd-Row-&quot; + i);
                }
                else if(i &lt; 10)
                {
                    Assert.AreEqual(0, cells.Rows[i].GroupLevel, &quot;CoverLastEnd-Row.GroupLevel-&quot; + i);
                    Assert.AreEqual(13 - i, cells[i, 0].IntValue, &quot;CoverLastEnd-Row-&quot; + i);
                }
                else
                {
                    Assert.AreEqual(i &lt; 13 ? 1 : 0, cells.Rows[i].GroupLevel, &quot;CoverLastEnd-Row.GroupLevel-&quot; + i);
                    Assert.AreEqual(i - 10, cells[i, 0].IntValue, &quot;CoverLastEnd-Row-&quot; + i);
                }
            }

            cells.Clear();
            for (int i = 0; i &lt; 14; i++)
            {
                cells[i, 0].PutValue(i);
            }
            cells.GroupRows(0, 2);
            cells.GroupRows(7, 12);
            sorter.Sort(cells, 2, 0, 12, 0);
            for (int i = 0; i &lt; 14; i++)
            {
                if (i &gt; 6)
                {
                    Assert.AreEqual(i &lt; 13 ? 1 : 0, cells.Rows[i].GroupLevel, &quot;ExcludeLastEnd-Row.GroupLevel-&quot; + i);
                    Assert.AreEqual(i, cells[i, 0].IntValue, &quot;ExcludeLastEnd-Row-&quot; + i);
                }
                else if (i &lt; 3)
                {
                    Assert.AreEqual(0, cells.Rows[i].GroupLevel, &quot;ExcludeLastEnd-Row.GroupLevel-&quot; + i);
                    Assert.AreEqual(6 - i, cells[i, 0].IntValue, &quot;ExcludeLastEnd-Row-&quot; + i);
                }
                else
                {
                    Assert.AreEqual(i &lt; 6 ? 1 : 0, cells.Rows[i].GroupLevel, &quot;ExcludeLastEnd-Row.GroupLevel-&quot; + i);
                    Assert.AreEqual(i - 3, cells[i, 0].IntValue, &quot;ExcludeLastEnd-Row-&quot; + i);
                }
            }

            int[] vals = new int[] { 1, 2, 3, 8, 5, 6, 7, 9, 4, 10, 11, 12, 13, 14, };
            cells.Clear();
            for (int i = 0; i &lt; vals.Length; i++)
            {
                cells[i, 0].PutValue(vals[i]);
            }
            cells.GroupRows(0, 2);
            cells.GroupRows(4, 6);
            cells.GroupRows(8, 10);
            sorter.Sort(cells, 0, 0, 13, 0);
            vals = new int[] { 14, 13, 4, 10, 11, 12, 5, 6, 7, 9, 1, 2, 3, 8, };
            for (int i = 0; i &lt; 14; i++)
            {
                Assert.AreEqual(vals[i], cells[i, 0].IntValue, &quot;ParallelGroup-Row-&quot; + i);
            }

            cells.Clear();
            vals = new int[] { 1, 2, 3, 4, 13, 6, 7, 8, 9, 5, 11, 12, 10, 14, };
            for (int i = 0; i &lt; vals.Length; i++)
            {
                cells[i, 0].PutValue(vals[i]);
            }
            cells.GroupRows(0, 1);
            cells.GroupRows(0, 3);
            cells.GroupRows(6, 7);
            cells.GroupRows(5, 8);
            cells.GroupRows(10, 11);
            sorter.Sort(cells, 0, 0, 13, 0);
            vals = new int[] { 14, 1, 2, 3, 4, 13, 11, 12, 10, 6, 7, 8, 9, 5, };
            for (int i = 0; i &lt; 14; i++)
            {
                Assert.AreEqual(vals[i], cells[i, 0].IntValue, &quot;ParallelSub-Row-&quot; + i);
            }

            cells.Clear();
            vals = new int[] { 1, 2, 3, 4, 13, 6, 7, 8, 9, 5, 11, 12, 10, 14, };
            for (int i = 0; i &lt; vals.Length; i++)
            {
                cells[i, 0].PutValue(vals[i]);
            }
            cells.GroupRows(0, 1);
            cells.GroupRows(0, 3);
            cells.GroupRows(6, 7);
            cells.GroupRows(5, 8);
            cells.GroupRows(10, 11);
            sorter.Sort(cells, 0, 0, 13, 0);
            vals = new int[] { 14, 1, 2, 3, 4, 13, 11, 12, 10, 6, 7, 8, 9, 5, };
            for (int i = 0; i &lt; 14; i++)
            {
                Assert.AreEqual(vals[i], cells[i, 0].IntValue, &quot;DiffSub-Row-&quot; + i);
            }

            cells.Clear();
            for (int i = 0; i &lt; 14; i++)
            {
                cells[i, 0].PutValue(i);
            }
            cells.GroupRows(2, 3);
            cells.GroupRows(7, 12);
            sorter.Sort(cells, 0, 0, 10, 0);
            for (int i = 0; i &lt; 14; i++)
            {
                Assert.AreEqual(i &gt;= 2 &amp;&amp; i &lt;= 3 || i &gt;= 7 &amp;&amp; i &lt;= 12 ? 1 : 0, cells.Rows[i].GroupLevel,
                    &quot;NoStart-Row.OutlineLevel-&quot; + i);
                Assert.AreEqual(i &lt; 11 ? 10 - i : i, cells[i, 0].IntValue, &quot;NoStart-Row-&quot; + i);
            }

            cells.Clear();
            for (int i = 0; i &lt; 14; i++)
            {
                cells[i, 0].PutValue(i);
            }
            cells.GroupRows(2, 3);
            cells.GroupRows(7, 12);
            cells.GroupRows(0, 13);
            sorter.Sort(cells, 0, 0, 10, 0);
            vals = new int[] { 6, 5, 2, 3, 4, 1, 0, 7, 8, 9, 10, 11, 12, 13, };
            for (int i = 0; i &lt; 14; i++)
            {
                Assert.AreEqual(i &gt;= 2 &amp;&amp; i &lt;= 3 || i &gt;= 7 &amp;&amp; i &lt;= 12 ? 2 : 1, cells.Rows[i].GroupLevel,
                    &quot;InGroupNoStart-Row.OutlineLevel-&quot; + i);
                Assert.AreEqual(vals[i], cells[i, 0].IntValue, &quot;InGroupNoStart-Row-&quot; + i);
            }

            sorter.SortLeftToRight = true;
            cells.Clear();
            cells.Columns.Clear();
            for (int i = 0; i &lt; 14; i++)
            {
                cells[0, i].PutValue(i);
            }
            cells.GroupColumns(0, 2);
            sorter.Sort(cells, 0, 3, 0, 13);
            for (int i = 0; i &lt; 14; i++)
            {
                Assert.AreEqual(i &lt; 3 ? i : 16 - i, cells[0, i].IntValue, &quot;FromEnd-Column-&quot; + i);
            }

            cells.Clear();
            cells.Columns.Clear();
            for (int i = 0; i &lt; 14; i++)
            {
                cells[0, i].PutValue(i);
            }
            cells.GroupColumns(0, 2);
            sorter.Sort(cells, 0, 2, 0, 13);
            for (int i = 0; i &lt; 14; i++)
            {
                Assert.AreEqual(i &lt; 10 ? 13 - i : i - 10, cells[0, i].IntValue, &quot;FromPartial-Column-&quot; + i);
            }

            cells.Clear();
            cells.Columns.Clear();
            cells.Columns[0].Width = 2; //CELLSJAVA-45402
            for (int i = 0; i &lt; 14; i++)
            {
                cells[0, i].PutValue(i);
            }
            cells.GroupColumns(1, 2);
            sorter.Sort(cells, 0, 2, 0, 13);
            Assert.AreEqual(0, cells[0, 0].IntValue, &quot;FromPartial-Column-0&quot;);
            for (int i = 1; i &lt; 14; i++)
            {
                Assert.AreEqual(i &lt; 11 ? 14 - i : i - 10, cells[0, i].IntValue, &quot;FromPartial-Column-&quot; + i);
            }

            cells.Clear();
            cells.Columns.Clear();
            for (int i = 0; i &lt; 14; i++)
            {
                cells[0, i].PutValue(i);
            }
            cells.GroupColumns(0, 2);
            cells.GroupColumns(0, 4);
            sorter.Sort(cells, 0, 2, 0, 13);
            for (int i = 0; i &lt; 14; i++)
            {
                Assert.AreEqual(i &lt; 8 ? 13 - i : i - 8, cells[0, i].IntValue, &quot;FromPartialInSub-Column-&quot; + i);
            }

            cells.Clear();
            cells.Columns.Clear();
            for (int i = 0; i &lt; 14; i++)
            {
                cells[0, i].PutValue(i);
            }
            cells.GroupColumns(0, 2);
            cells.GroupColumns(0, 4);
            sorter.Sort(cells, 0, 3, 0, 13);
            for (int i = 0; i &lt; 14; i++)
            {
                Assert.AreEqual(i &lt; 8 ? 13 - i : i - 8, cells[0, i].IntValue, &quot;FromPartialAfterSub-Column-&quot; + i);
            }

            cells.Clear();
            cells.Columns.Clear();
            for (int i = 0; i &lt; 14; i++)
            {
                cells[0, i].PutValue(i);
            }
            cells.GroupColumns(0, 2);
            cells.GroupColumns(0, 13);
            sorter.Sort(cells, 0, 2, 0, 13);
            for (int i = 0; i &lt; 14; i++)
            {
                Assert.AreEqual(i &lt; 10 ? 13 - i : i - 10, cells[0, i].IntValue, &quot;WithinGroup-Column-&quot; + i);
            }

            cells.Clear();
            cells.Columns.Clear();
            for (int i = 0; i &lt; 14; i++)
            {
                cells[0, i].PutValue(i);
            }
            cells.GroupColumns(0, 2);
            cells.GroupColumns(7, 12);
            sorter.Sort(cells, 0, 2, 0, 13);
            for (int i = 0; i &lt; 14; i++)
            {
                Assert.AreEqual(i &lt; 7 ? i + 7 : (i &lt; 10 ? 13 - i : i - 10), cells[0, i].IntValue, &quot;CoverLastEnd-Column-&quot; + i);
            }

            cells.Clear();
            cells.Columns.Clear();
            for (int i = 0; i &lt; 14; i++)
            {
                cells[0, i].PutValue(i);
            }
            cells.GroupColumns(0, 2);
            cells.GroupColumns(7, 12);
            sorter.Sort(cells, 0, 2, 0, 12);
            for (int i = 0; i &lt; 14; i++)
            {
                Assert.AreEqual(i &lt; 3 ? 6 - i : (i &lt; 7 ? i - 3 : i), cells[0, i].IntValue, &quot;ExcludeLastEnd-Column-&quot; + i);
            }

            vals = new int[] { 1, 2, 3, 8, 5, 6, 7, 9, 4, 10, 11, 12, 13, 14, };
            cells.Clear();
            cells.Columns.Clear();
            for (int i = 0; i &lt; vals.Length; i++)
            {
                cells[0, i].PutValue(vals[i]);
            }
            cells.GroupColumns(0, 2);
            cells.GroupColumns(4, 6);
            cells.GroupColumns(8, 10);
            sorter.Sort(cells, 0, 0, 0, 13);
            vals = new int[] { 14, 13, 4, 10, 11, 12, 5, 6, 7, 9, 1, 2, 3, 8, };
            for (int i = 0; i &lt; 14; i++)
            {
                Assert.AreEqual(vals[i], cells[0, i].IntValue, &quot;ParallelGroup-Column-&quot; + i);
            }

            cells.Clear();
            cells.Columns.Clear();
            vals = new int[] { 1, 2, 3, 4, 13, 6, 7, 8, 9, 5, 11, 12, 10, 14, };
            for (int i = 0; i &lt; vals.Length; i++)
            {
                cells[0, i].PutValue(vals[i]);
            }
            cells.GroupColumns(0, 1);
            cells.GroupColumns(0, 3);
            cells.GroupColumns(6, 7);
            cells.GroupColumns(5, 8);
            cells.GroupColumns(10, 11);
            sorter.Sort(cells, 0, 0, 0, 13);
            vals = new int[] { 14, 1, 2, 3, 4, 13, 11, 12, 10, 6, 7, 8, 9, 5, };
            for (int i = 0; i &lt; 14; i++)
            {
                Assert.AreEqual(vals[i], cells[0, i].IntValue, &quot;ParallelSub-Column-&quot; + i);
            }

            cells.Clear();
            cells.Columns.Clear();
            vals = new int[] { 1, 2, 3, 4, 13, 6, 7, 8, 9, 5, 11, 12, 10, 14, };
            for (int i = 0; i &lt; vals.Length; i++)
            {
                cells[0, i].PutValue(vals[i]);
            }
            cells.GroupColumns(0, 1);
            cells.GroupColumns(0, 3);
            cells.GroupColumns(6, 7);
            cells.GroupColumns(5, 8);
            cells.GroupColumns(10, 11);
            sorter.Sort(cells, 0, 0, 0, 13);
            vals = new int[] { 14, 1, 2, 3, 4, 13, 11, 12, 10, 6, 7, 8, 9, 5, };
            for (int i = 0; i &lt; 14; i++)
            {
                Assert.AreEqual(vals[i], cells[0, i].IntValue, &quot;DiffSub-Column-&quot; + i);
            }
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


