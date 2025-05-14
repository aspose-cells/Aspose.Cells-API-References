---
title: Cells.GroupRows
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Groups rows
type: docs
url: /net/aspose.cells/cells/grouprows/
---
## GroupRows(int, int, bool) {#grouprows_1}

Groups rows.

```csharp
public void GroupRows(int firstIndex, int lastIndex, bool isHidden)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | The first row index to be grouped. |
| lastIndex | Int32 | The last row index to be grouped. |
| isHidden | Boolean | Specifies if the grouped rows are hidden. |

### Examples

```csharp
// Called: cells.GroupRows((i * 10 + 1), (i * 10 + 9), true);
public void Cells_Method_GroupRows()
{
    Workbook wb = new Workbook();
    Worksheet sheet = wb.Worksheets[0];
    Cells cells = sheet.Cells;
    Random rdm = new Random();
    for (int i = 0; i < 200; i++)
    {
        int index = (int)(rdm.NextDouble() * 100);
        string columnName = CellsHelper.ColumnIndexToName(index);
        for (int j = 1; j < 10; j++)
        {
            cells["A" + (i * 10 + j)].PutValue(columnName + "A" + i);
            cells["B" + (i * 10 + j)].PutValue(columnName + "B" +(index * 10 + j));
            cells["C" + (i * 10 + j)].PutValue(columnName + "C" + j);
            cells["D" + (i * 10 + j)].PutValue(columnName + "D" +(i * 10 + j));
        }
        cells.GroupRows((i * 10 + 1), (i * 10 + 9), true);
    }
    sheet.Outline.SummaryRowBelow = false;
    DataSorter sorter = wb.DataSorter;
    sorter.AddKey(2, SortOrder.Ascending);
    sorter.AddKey(0, SortOrder.Descending);
    sorter.AddKey(1, SortOrder.Descending);
    sorter.Sort(cells, 0, 0, 2000, 4); //here should not give exception
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GroupRows(int, int) {#grouprows}

Groups rows.

```csharp
public void GroupRows(int firstIndex, int lastIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | The first row index to be grouped. |
| lastIndex | Int32 | The last row index to be grouped. |

### Examples

```csharp
// Called: cells.GroupRows(1048575, 1048575);
public void Cells_Method_GroupRows()
{
    caseName = "testGroupRows_Excel2007_002";
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Cells cells = workbook.Worksheets[0].Cells;
    cells.GroupRows(1048575, 1048575);

    workbook.Save(Constants.destPath + "testGroupRows.xlsx");
    workbook = new Workbook(Constants.destPath + "testGroupRows.xlsx");
    workbook.Save(Constants.destPath + "testGroupRows.xls");
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


