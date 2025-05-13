---
title: DataSorter.Sort
second_title: Aspose.Cells for .NET API Reference
description: DataSorter method. Sorts the data of the area
type: docs
url: /net/aspose.cells/datasorter/sort/
---
## Sort(Cells, int, int, int, int) {#sort_2}

Sorts the data of the area.

```csharp
public int[] Sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cells | Cells | The cells contains the data area. |
| startRow | Int32 | The start row of the area. |
| startColumn | Int32 | The start column of the area. |
| endRow | Int32 | The end row of the area. |
| endColumn | Int32 | The end column of the area. |

### Return Value

the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.

### Examples

```csharp
// Called: sorter.Sort(cells, 0, 0, 5, 0);
public void DataSorter_Method_Sort()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i < 6; i++)
            {
                cells[i, 0].PutValue(6 - i);
            }
            cells.Rows[1].IsHidden = true;
            DataSorter sorter = wb.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);
            sorter.Sort(cells, 0, 0, 5, 0);
            Assert.AreEqual(1, cells[0, 0].IntValue, "A1");
            Assert.AreEqual(5, cells[1, 0].IntValue, "A2");
            Assert.IsTrue(cells.Rows[1].IsHidden, "The second row should be hidden and should not be sorted");
            Assert.AreEqual(2, cells[2, 0].IntValue, "A3");
            Assert.AreEqual(3, cells[3, 0].IntValue, "A4");
            Assert.AreEqual(4, cells[4, 0].IntValue, "A5");
            Assert.AreEqual(6, cells[5, 0].IntValue, "A6");
        }
```

### See Also

* class [Cells](../../cells/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Sort(Cells, CellArea) {#sort_1}

Sort the data of the area.

```csharp
public int[] Sort(Cells cells, CellArea area)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cells | Cells | The cells contains the data area. |
| area | CellArea | The area needed to sort |

### Return Value

the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.

### Examples

```csharp
// Called: dataSorter.Sort(workbook.Worksheets[0].Cells, ca);
public void DataSorter_Method_Sort()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");

    workbook.Worksheets[0].Cells.GroupRows(1, 2, false);

    DataSorter dataSorter = workbook.DataSorter;
    dataSorter.HasHeaders = true;

    CellArea ca = new CellArea();

    dataSorter.Key1 = 0;

    dataSorter.Order1 = Aspose.Cells.SortOrder.Descending;

    ca.StartRow = 0;

    ca.StartColumn = 0;

    ca.EndColumn = 1;

    ca.EndRow = 12;

    dataSorter.Sort(workbook.Worksheets[0].Cells, ca);
    Assert.AreEqual(workbook.Worksheets[0].Cells["A10"].StringValue, "1996");

    workbook.Save(Constants.destPath + "example.xls");
}
```

### See Also

* class [Cells](../../cells/)
* struct [CellArea](../../cellarea/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Sort() {#sort}

Sort the data in the range.

```csharp
public int[] Sort()
```

### Return Value

the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.

### Examples

```csharp
// Called: tableList.AutoFilter.Sorter.Sort();
public void DataSorter_Method_Sort()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "Sort/SortDataTemplate.xltx");
    Worksheet currentSheet = workbook.Worksheets[0];
    Aspose.Cells.Tables.ListObject tableList = currentSheet.ListObjects["Table1"];
    tableList.AutoFilter.Sorter.Sort();
    Assert.IsTrue(currentSheet.Cells["C3"].IsFormula);
    Util.ReSave(workbook, SaveFormat.Xlsx);
}
```

### See Also

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


