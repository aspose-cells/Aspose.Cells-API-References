---
title: Cells.Clear
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Clears all data of the worksheet
type: docs
url: /net/aspose.cells/cells/clear/
---
## Cells.Clear method

Clears all data of the worksheet.

```csharp
public void Clear()
```

### Examples

```csharp
// Called: cells.Clear();
[Test]
        public void Method_Clear()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            DataSorter sorter = wb.DataSorter;
            sorter.AddKey(0, SortOrder.Descending);

            for (int i = 0; i < 14; i++)
            {
                cells[i, 0].PutValue(i);
            }
            cells.GroupRows(0, 2);
            sorter.Sort(cells, 3, 0, 13, 0);
            for (int i = 0; i < 14; i++)
            {
                if (i < 3)
                {
                    Assert.AreEqual(1, cells.Rows[i].GroupLevel, "FromEnd-Row.GroupLevel-" + i);
                    Assert.AreEqual(i, cells[i, 0].IntValue, "FromEnd-Row-" + i);
                }
                else
                {
                    Assert.AreEqual(0, cells.Rows[i].GroupLevel, "FromEnd-Row.GroupLevel-" + i);
                    Assert.AreEqual(16 - i, cells[i, 0].IntValue, "FromEnd-Row-" + i);
                }
            }

            cells.Clear();
            for (int i = 0; i < 14; i++)
            {
                cells[i, 0].PutValue(i);
            }
            cells.GroupRows(0, 2);
            sorter.Sort(cells, 2, 0, 13, 0);
            for (int i = 0; i < 14; i++)
            {
                if (i < 10)
                {
                    Assert.AreEqual(0, cells.Rows[i].GroupLevel, "FromPartial-Row.GroupLevel-" + i);
                    Assert.AreEqual(13 - i, cells[i, 0].IntValue, "FromPartial-Row-" + i);
                }
                else
                {
                    Assert.AreEqual(i < 13 ? 1 : 0, cells.Rows[i].GroupLevel, "FromPartial-Row.GroupLevel-" + i);
                    Assert.AreEqual(i - 10, cells[i, 0].IntValue, "FromPartial-Row-" + i);
                }
            }

            //CELLSJAVA-45402: first row should not be sorted
            cells.Clear();
            for (int i = 0; i < 14; i++)
            {
                cells[i, 0].PutValue(i);
            }
            cells.GroupRows(1, 2);
            sorter.Sort(cells, 2, 0, 13, 0);
            Assert.AreEqual(0, cells.Rows[0].GroupLevel, "FromPartial-Row.GroupLevel-0");
            Assert.AreEqual(0, cells[0, 0].IntValue, "FromPartial-Row-0");
            for (int i = 1; i < 14; i++)
            {
                if (i < 11)
                {
                    Assert.AreEqual(0, cells.Rows[i].GroupLevel, "FromPartial-Row.GroupLevel-" + i);
                    Assert.AreEqual(14 - i, cells[i, 0].IntValue, "FromPartial-Row-" + i);
                }
                else
                {
                    Assert.AreEqual(i < 13 ? 1 : 0, cells.Rows[i].GroupLevel, "FromPartial-Row.GroupLevel-" + i);
                    Assert.AreEqual(i - 10, cells[i, 0].IntValue, "FromPartial-Row-" + i);
                }
            }

            cells.Clear();
            for (int i = 0; i < 14; i++)
            {
                cells[i, 0].PutValue(i);
            }
            cells.GroupRows(0, 2);
            cells.GroupRows(0, 4);
            sorter.Sort(cells, 2, 0, 13, 0);
            for (int i = 0; i < 14; i++)
            {
                if (i < 8)
                {
                    Assert.AreEqual(0, cells.Rows[i].GroupLevel, "FromPartialInSub-Row.GroupLevel-" + i);
                    Assert.AreEqual(13 - i, cells[i, 0].IntValue, "FromPartialInSub-Row-" + i);
                }
                else
                {
                    Assert.AreEqual(i < 11 ? 2 : (i < 13 ? 1 : 0), cells.Rows[i].GroupLevel,
                        "FromPartialInSub-Row.GroupLevel-" + i);
                    Assert.AreEqual(i - 8, cells[i, 0].IntValue, "FromPartialInSub-Row-" + i);
                }
            }

            cells.Clear();
            for (int i = 0; i < 14; i++)
            {
                cells[i, 0].PutValue(i);
            }
            cells.GroupRows(0, 2);
            cells.GroupRows(0, 4);
            sorter.Sort(cells, 3, 0, 13, 0);
            for (int i = 0; i < 14; i++)
            {
                if (i < 8)
                {
                    Assert.AreEqual(0, cells.Rows[i].GroupLevel, "FromPartialAfterSub-Row.GroupLevel-" + i);
                    Assert.AreEqual(13 - i, cells[i, 0].IntValue, "FromPartialAfterSub-Row-" + i);
                }
                else
                {
                    Assert.AreEqual(i < 11 ? 2 : (i < 13 ? 1 : 0), cells.Rows[i].GroupLevel,
                        "FromPartialAfterSub-Row.GroupLevel-" + i);
                    Assert.AreEqual(i - 8, cells[i, 0].IntValue, "FromPartialAfterSub-Row-" + i);
                }
            }

            cells.Clear();
            for (int i = 0; i < 14; i++)
            {
                cells[i, 0].PutValue(i);
            }
            cells.GroupRows(0, 2);
            cells.GroupRows(0, 13);
            sorter.Sort(cells, 2, 0, 13, 0);
            for (int i = 0; i < 14; i++)
            {
                if (i < 10)
                {
                    Assert.AreEqual(1, cells.Rows[i].GroupLevel, "WithinGroup-Row.GroupLevel-" + i);
                    Assert.AreEqual(13 - i, cells[i, 0].IntValue, "WithinGroup-Row-" + i);
                }
                else
                {
                    Assert.AreEqual(i < 13 ? 2 : 1, cells.Rows[i].GroupLevel, "WithinGroup-Row.GroupLevel-" + i);
                    Assert.AreEqual(i - 10, cells[i, 0].IntValue, "WithinGroup-Row-" + i);
                }
            }

            cells.Clear();
            for (int i = 0; i < 14; i++)
            {
                cells[i, 0].PutValue(i);
            }
            cells.GroupRows(0, 2);
            cells.GroupRows(7, 12);
            sorter.Sort(cells, 2, 0, 13, 0);
            for (int i = 0; i < 14; i++)
            {
                if (i < 7)
                {
                    Assert.AreEqual(i < 6 ? 1 : 0, cells.Rows[i].GroupLevel, "CoverLastEnd-Row.GroupLevel-" + i);
                    Assert.AreEqual(i + 7, cells[i, 0].IntValue, "CoverLastEnd-Row-" + i);
                }
                else if(i < 10)
                {
                    Assert.AreEqual(0, cells.Rows[i].GroupLevel, "CoverLastEnd-Row.GroupLevel-" + i);
                    Assert.AreEqual(13 - i, cells[i, 0].IntValue, "CoverLastEnd-Row-" + i);
                }
                else
                {
                    Assert.AreEqual(i < 13 ? 1 : 0, cells.Rows[i].GroupLevel, "CoverLastEnd-Row.GroupLevel-" + i);
                    Assert.AreEqual(i - 10, cells[i, 0].IntValue, "CoverLastEnd-Row-" + i);
                }
            }

            cells.Clear();
            for (int i = 0; i < 14; i++)
            {
                cells[i, 0].PutValue(i);
            }
            cells.GroupRows(0, 2);
            cells.GroupRows(7, 12);
            sorter.Sort(cells, 2, 0, 12, 0);
            for (int i = 0; i < 14; i++)
            {
                if (i > 6)
                {
                    Assert.AreEqual(i < 13 ? 1 : 0, cells.Rows[i].GroupLevel, "ExcludeLastEnd-Row.GroupLevel-" + i);
                    Assert.AreEqual(i, cells[i, 0].IntValue, "ExcludeLastEnd-Row-" + i);
                }
                else if (i < 3)
                {
                    Assert.AreEqual(0, cells.Rows[i].GroupLevel, "ExcludeLastEnd-Row.GroupLevel-" + i);
                    Assert.AreEqual(6 - i, cells[i, 0].IntValue, "ExcludeLastEnd-Row-" + i);
                }
                else
                {
                    Assert.AreEqual(i < 6 ? 1 : 0, cells.Rows[i].GroupLevel, "ExcludeLastEnd-Row.GroupLevel-" + i);
                    Assert.AreEqual(i - 3, cells[i, 0].IntValue, "ExcludeLastEnd-Row-" + i);
                }
            }

            int[] vals = new int[] { 1, 2, 3, 8, 5, 6, 7, 9, 4, 10, 11, 12, 13, 14, };
            cells.Clear();
            for (int i = 0; i < vals.Length; i++)
            {
                cells[i, 0].PutValue(vals[i]);
            }
            cells.GroupRows(0, 2);
            cells.GroupRows(4, 6);
            cells.GroupRows(8, 10);
            sorter.Sort(cells, 0, 0, 13, 0);
            vals = new int[] { 14, 13, 4, 10, 11, 12, 5, 6, 7, 9, 1, 2, 3, 8, };
            for (int i = 0; i < 14; i++)
            {
                Assert.AreEqual(vals[i], cells[i, 0].IntValue, "ParallelGroup-Row-" + i);
            }

            cells.Clear();
            vals = new int[] { 1, 2, 3, 4, 13, 6, 7, 8, 9, 5, 11, 12, 10, 14, };
            for (int i = 0; i < vals.Length; i++)
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
            for (int i = 0; i < 14; i++)
            {
                Assert.AreEqual(vals[i], cells[i, 0].IntValue, "ParallelSub-Row-" + i);
            }

            cells.Clear();
            vals = new int[] { 1, 2, 3, 4, 13, 6, 7, 8, 9, 5, 11, 12, 10, 14, };
            for (int i = 0; i < vals.Length; i++)
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
            for (int i = 0; i < 14; i++)
            {
                Assert.AreEqual(vals[i], cells[i, 0].IntValue, "DiffSub-Row-" + i);
            }

            cells.Clear();
            for (int i = 0; i < 14; i++)
            {
                cells[i, 0].PutValue(i);
            }
            cells.GroupRows(2, 3);
            cells.GroupRows(7, 12);
            sorter.Sort(cells, 0, 0, 10, 0);
            for (int i = 0; i < 14; i++)
            {
                Assert.AreEqual(i >= 2 && i <= 3 || i >= 7 && i <= 12 ? 1 : 0, cells.Rows[i].GroupLevel,
                    "NoStart-Row.OutlineLevel-" + i);
                Assert.AreEqual(i < 11 ? 10 - i : i, cells[i, 0].IntValue, "NoStart-Row-" + i);
            }

            cells.Clear();
            for (int i = 0; i < 14; i++)
            {
                cells[i, 0].PutValue(i);
            }
            cells.GroupRows(2, 3);
            cells.GroupRows(7, 12);
            cells.GroupRows(0, 13);
            sorter.Sort(cells, 0, 0, 10, 0);
            vals = new int[] { 6, 5, 2, 3, 4, 1, 0, 7, 8, 9, 10, 11, 12, 13, };
            for (int i = 0; i < 14; i++)
            {
                Assert.AreEqual(i >= 2 && i <= 3 || i >= 7 && i <= 12 ? 2 : 1, cells.Rows[i].GroupLevel,
                    "InGroupNoStart-Row.OutlineLevel-" + i);
                Assert.AreEqual(vals[i], cells[i, 0].IntValue, "InGroupNoStart-Row-" + i);
            }

            sorter.SortLeftToRight = true;
            cells.Clear();
            cells.Columns.Clear();
            for (int i = 0; i < 14; i++)
            {
                cells[0, i].PutValue(i);
            }
            cells.GroupColumns(0, 2);
            sorter.Sort(cells, 0, 3, 0, 13);
            for (int i = 0; i < 14; i++)
            {
                Assert.AreEqual(i < 3 ? i : 16 - i, cells[0, i].IntValue, "FromEnd-Column-" + i);
            }

            cells.Clear();
            cells.Columns.Clear();
            for (int i = 0; i < 14; i++)
            {
                cells[0, i].PutValue(i);
            }
            cells.GroupColumns(0, 2);
            sorter.Sort(cells, 0, 2, 0, 13);
            for (int i = 0; i < 14; i++)
            {
                Assert.AreEqual(i < 10 ? 13 - i : i - 10, cells[0, i].IntValue, "FromPartial-Column-" + i);
            }

            cells.Clear();
            cells.Columns.Clear();
            cells.Columns[0].Width = 2; //CELLSJAVA-45402
            for (int i = 0; i < 14; i++)
            {
                cells[0, i].PutValue(i);
            }
            cells.GroupColumns(1, 2);
            sorter.Sort(cells, 0, 2, 0, 13);
            Assert.AreEqual(0, cells[0, 0].IntValue, "FromPartial-Column-0");
            for (int i = 1; i < 14; i++)
            {
                Assert.AreEqual(i < 11 ? 14 - i : i - 10, cells[0, i].IntValue, "FromPartial-Column-" + i);
            }

            cells.Clear();
            cells.Columns.Clear();
            for (int i = 0; i < 14; i++)
            {
                cells[0, i].PutValue(i);
            }
            cells.GroupColumns(0, 2);
            cells.GroupColumns(0, 4);
            sorter.Sort(cells, 0, 2, 0, 13);
            for (int i = 0; i < 14; i++)
            {
                Assert.AreEqual(i < 8 ? 13 - i : i - 8, cells[0, i].IntValue, "FromPartialInSub-Column-" + i);
            }

            cells.Clear();
            cells.Columns.Clear();
            for (int i = 0; i < 14; i++)
            {
                cells[0, i].PutValue(i);
            }
            cells.GroupColumns(0, 2);
            cells.GroupColumns(0, 4);
            sorter.Sort(cells, 0, 3, 0, 13);
            for (int i = 0; i < 14; i++)
            {
                Assert.AreEqual(i < 8 ? 13 - i : i - 8, cells[0, i].IntValue, "FromPartialAfterSub-Column-" + i);
            }

            cells.Clear();
            cells.Columns.Clear();
            for (int i = 0; i < 14; i++)
            {
                cells[0, i].PutValue(i);
            }
            cells.GroupColumns(0, 2);
            cells.GroupColumns(0, 13);
            sorter.Sort(cells, 0, 2, 0, 13);
            for (int i = 0; i < 14; i++)
            {
                Assert.AreEqual(i < 10 ? 13 - i : i - 10, cells[0, i].IntValue, "WithinGroup-Column-" + i);
            }

            cells.Clear();
            cells.Columns.Clear();
            for (int i = 0; i < 14; i++)
            {
                cells[0, i].PutValue(i);
            }
            cells.GroupColumns(0, 2);
            cells.GroupColumns(7, 12);
            sorter.Sort(cells, 0, 2, 0, 13);
            for (int i = 0; i < 14; i++)
            {
                Assert.AreEqual(i < 7 ? i + 7 : (i < 10 ? 13 - i : i - 10), cells[0, i].IntValue, "CoverLastEnd-Column-" + i);
            }

            cells.Clear();
            cells.Columns.Clear();
            for (int i = 0; i < 14; i++)
            {
                cells[0, i].PutValue(i);
            }
            cells.GroupColumns(0, 2);
            cells.GroupColumns(7, 12);
            sorter.Sort(cells, 0, 2, 0, 12);
            for (int i = 0; i < 14; i++)
            {
                Assert.AreEqual(i < 3 ? 6 - i : (i < 7 ? i - 3 : i), cells[0, i].IntValue, "ExcludeLastEnd-Column-" + i);
            }

            vals = new int[] { 1, 2, 3, 8, 5, 6, 7, 9, 4, 10, 11, 12, 13, 14, };
            cells.Clear();
            cells.Columns.Clear();
            for (int i = 0; i < vals.Length; i++)
            {
                cells[0, i].PutValue(vals[i]);
            }
            cells.GroupColumns(0, 2);
            cells.GroupColumns(4, 6);
            cells.GroupColumns(8, 10);
            sorter.Sort(cells, 0, 0, 0, 13);
            vals = new int[] { 14, 13, 4, 10, 11, 12, 5, 6, 7, 9, 1, 2, 3, 8, };
            for (int i = 0; i < 14; i++)
            {
                Assert.AreEqual(vals[i], cells[0, i].IntValue, "ParallelGroup-Column-" + i);
            }

            cells.Clear();
            cells.Columns.Clear();
            vals = new int[] { 1, 2, 3, 4, 13, 6, 7, 8, 9, 5, 11, 12, 10, 14, };
            for (int i = 0; i < vals.Length; i++)
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
            for (int i = 0; i < 14; i++)
            {
                Assert.AreEqual(vals[i], cells[0, i].IntValue, "ParallelSub-Column-" + i);
            }

            cells.Clear();
            cells.Columns.Clear();
            vals = new int[] { 1, 2, 3, 4, 13, 6, 7, 8, 9, 5, 11, 12, 10, 14, };
            for (int i = 0; i < vals.Length; i++)
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
            for (int i = 0; i < 14; i++)
            {
                Assert.AreEqual(vals[i], cells[0, i].IntValue, "DiffSub-Column-" + i);
            }
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


