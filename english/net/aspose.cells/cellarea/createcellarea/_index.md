---
title: CellArea.CreateCellArea
second_title: Aspose.Cells for .NET API Reference
description: CellArea method. Creates a cell area
type: docs
url: /net/aspose.cells/cellarea/createcellarea/
---
## CreateCellArea(int, int, int, int) {#createcellarea}

Creates a cell area.

```csharp
public static CellArea CreateCellArea(int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The start row. |
| startColumn | Int32 | The start column. |
| endRow | Int32 | The end row. |
| endColumn | Int32 | The end column. |

### Return Value

Return a [`CellArea`](../).

### Examples

```csharp
// Called: sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 8, 2));
public void CellArea_Method_CreateCellArea()
{
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets[0].Cells;
    int[] vs = new int[] { 1, 3, 2, 6, 4, 5, 8, 9, 7 };
    for (int i = 0; i < vs.Length; i++)
    {
        cells[i, i / 3].PutValue(vs[i]);
    }
    DataSorter sorter = wb.DataSorter;
    sorter.Clear();
    sorter.Order1 = SortOrder.Ascending;
    sorter.Key1 = 2;
    sorter.Order2 = SortOrder.Ascending;
    sorter.Key2 = 1;
    sorter.Order3 = SortOrder.Ascending;
    sorter.Key3 = 0;
    sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 8, 2));
    vs = new int[] { 7, 8, 9, 4, 5, 6, 1, 2, 3 };
    for (int i = 0; i < vs.Length; i++)
    {
        Cell cell = cells[i, 2 - i / 3];
        Assert.AreEqual(vs[i], cell.IntValue, cell.Name);
    }
}
```

### See Also

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateCellArea(string, string) {#createcellarea_1}

Creates a cell area.

```csharp
public static CellArea CreateCellArea(string startCellName, string endCellName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startCellName | String | The top-left cell of the range. |
| endCellName | String | The bottom-right cell of the range. |

### Return Value

Return a [`CellArea`](../).

### Examples

```csharp
// Called: CellArea ca = CellArea.CreateCellArea("B1","B100");
public void CellArea_Method_CreateCellArea()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    for (int i = 0; i < 100; i++)
    {
        cells[i, 0].PutValue(i);
    }
    CellArea ca = CellArea.CreateCellArea("B1","B100");
    cells.InsertRange(ca, ShiftType.Down);
    Assert.AreEqual(cells.Rows.Count, 100);
            
}
```

### See Also

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


