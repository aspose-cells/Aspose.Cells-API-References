---
title: Cells.UngroupRows
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Ungroups rows
type: docs
url: /net/aspose.cells/cells/ungrouprows/
---
## UngroupRows(int, int, bool) {#ungrouprows_1}

Ungroups rows.

```csharp
public void UngroupRows(int firstIndex, int lastIndex, bool isAll)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | The first row index to be ungrouped. |
| lastIndex | Int32 | The last row index to be ungrouped. |
| isAll | Boolean | True, removes all grouped info.Otherwise, remove the outer group info. |

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## UngroupRows(int, int) {#ungrouprows}

Ungroups rows.

```csharp
public void UngroupRows(int firstIndex, int lastIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | The first row index to be ungrouped. |
| lastIndex | Int32 | The last row index to be ungrouped. |

### Remarks

Only removes outer group info.

### Examples

```csharp
// Called: cells.UngroupRows(2, 4); //after sorting: 0--&amp;gt;2
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i &lt; 6; i++)
            {
                cells[i, 0].PutValue(i);
            }
            cells.GroupRows(0, 2);
            DataSorter sorter = wb.DataSorter;
            sorter.AddKey(0, SortOrder.Descending);
            int[] indices = sorter.Sort(cells, 0, 0, 5, 0);
            Assert.AreEqual(6, indices.Length, &quot;Length of sorted indices&quot;);
            Assert.AreEqual(5, cells[0, 0].IntValue, &quot;After sorting, A1&quot;);
            Assert.AreEqual(5, indices[0], &quot;Sorted indices[0]&quot;);
            Assert.AreEqual(4, cells[1, 0].IntValue, &quot;After sorting, A2&quot;);
            Assert.AreEqual(4, indices[1], &quot;Sorted indices[1]&quot;);
            for (int i = 0; i &lt; 4; i++)
            {
                Assert.AreEqual(i, cells[i + 2, 0].IntValue, &quot;After sorting, A&quot; + (i + 3));
                Assert.AreEqual(i, indices[i + 2], &quot;Sorted indices[&quot; + (i + 2) + &quot;]&quot;);
            }
            cells.UngroupRows(2, 4); //after sorting: 0--&gt;2

            for (int i = 0; i &lt; 6; i++)
            {
                cells[i, 0].PutValue(i);
            }
            cells.GroupRows(1, 3);
            indices = sorter.Sort(cells, 0, 0, 5, 0);
            Assert.AreEqual(6, indices.Length, &quot;Length of sorted indices&quot;);
            Assert.AreEqual(5, cells[0, 0].IntValue, &quot;After sorting, A1&quot;);
            Assert.AreEqual(5, indices[0], &quot;Sorted indices[0]&quot;);
            for (int i = 1; i &lt; 5; i++)
            {
                Assert.AreEqual(i, cells[i, 0].IntValue, &quot;After sorting, A&quot; + (i + 1));
                Assert.AreEqual(i, indices[i], &quot;Sorted indices[&quot; + i + &quot;]&quot;);
            }
            Assert.AreEqual(0, cells[5, 0].IntValue, &quot;After sorting, A6&quot;);
            Assert.AreEqual(0, indices[5], &quot;Sorted indices[5]&quot;);
            cells.UngroupRows(1, 3);

            for (int i = 0; i &lt; 6; i++)
            {
                cells[i, 0].PutValue(i);
            }
            cells.GroupRows(3, 4);
            indices = sorter.Sort(cells, 0, 0, 5, 0);
            Assert.AreEqual(6, indices.Length, &quot;Length of sorted indices&quot;);
            for (int i = 0; i &lt; 6; i++)
            {
                Assert.AreEqual(5 - i, cells[i, 0].IntValue, &quot;After sorting, A&quot; + (i + 1));
                Assert.AreEqual(5 - i, indices[i], &quot;Sorted indices[&quot; + i + &quot;]&quot;);
            }
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


