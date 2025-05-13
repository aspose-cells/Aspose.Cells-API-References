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
// Called: cells.UngroupRows(1, 3);
public void Cells_Method_UngroupRows()
{
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets[0].Cells;
    for (int i = 0; i < 6; i++)
    {
        cells[i, 0].PutValue(i);
    }
    cells.GroupRows(0, 2);
    DataSorter sorter = wb.DataSorter;
    sorter.AddKey(0, SortOrder.Descending);
    int[] indices = sorter.Sort(cells, 0, 0, 5, 0);
    Assert.AreEqual(6, indices.Length, "Length of sorted indices");
    Assert.AreEqual(5, cells[0, 0].IntValue, "After sorting, A1");
    Assert.AreEqual(5, indices[0], "Sorted indices[0]");
    Assert.AreEqual(4, cells[1, 0].IntValue, "After sorting, A2");
    Assert.AreEqual(4, indices[1], "Sorted indices[1]");
    for (int i = 0; i < 4; i++)
    {
        Assert.AreEqual(i, cells[i + 2, 0].IntValue, "After sorting, A" + (i + 3));
        Assert.AreEqual(i, indices[i + 2], "Sorted indices[" + (i + 2) + "]");
    }
    cells.UngroupRows(2, 4); //after sorting: 0-->2

    for (int i = 0; i < 6; i++)
    {
        cells[i, 0].PutValue(i);
    }
    cells.GroupRows(1, 3);
    indices = sorter.Sort(cells, 0, 0, 5, 0);
    Assert.AreEqual(6, indices.Length, "Length of sorted indices");
    Assert.AreEqual(5, cells[0, 0].IntValue, "After sorting, A1");
    Assert.AreEqual(5, indices[0], "Sorted indices[0]");
    for (int i = 1; i < 5; i++)
    {
        Assert.AreEqual(i, cells[i, 0].IntValue, "After sorting, A" + (i + 1));
        Assert.AreEqual(i, indices[i], "Sorted indices[" + i + "]");
    }
    Assert.AreEqual(0, cells[5, 0].IntValue, "After sorting, A6");
    Assert.AreEqual(0, indices[5], "Sorted indices[5]");
    cells.UngroupRows(1, 3);

    for (int i = 0; i < 6; i++)
    {
        cells[i, 0].PutValue(i);
    }
    cells.GroupRows(3, 4);
    indices = sorter.Sort(cells, 0, 0, 5, 0);
    Assert.AreEqual(6, indices.Length, "Length of sorted indices");
    for (int i = 0; i < 6; i++)
    {
        Assert.AreEqual(5 - i, cells[i, 0].IntValue, "After sorting, A" + (i + 1));
        Assert.AreEqual(5 - i, indices[i], "Sorted indices[" + i + "]");
    }
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


