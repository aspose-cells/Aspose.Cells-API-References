---
title: DataSorter.Key3
second_title: Aspose.Cells for .NET API Reference
description: DataSorter property. Represents third sorted column indexabsolute position column A is 0 B is 1 
type: docs
url: /net/aspose.cells/datasorter/key3/
---
## DataSorter.Key3 property

Represents third sorted column index(absolute position, column A is 0, B is 1, ...).

```csharp
public int Key3 { get; set; }
```

### Examples

```csharp
// Called: sorter.Key3 = 25;
public void DataSorter_Property_Key3()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet sheet = wb.Worksheets[0];
    Cells cells = sheet.Cells;
    DataSorter sorter = wb.DataSorter;
    sorter.Order1 = SortOrder.Ascending;
    sorter.Key1 = 4;
    sorter.Order2 = SortOrder.Ascending;
    sorter.Key2 = 5;
    sorter.Order3 = SortOrder.Ascending;
    sorter.Key3 = 6;
    sorter.Sort(cells, CellArea.CreateCellArea(7, 4, 15, 6));

    sorter.Clear();
    sorter.Order1 = SortOrder.Ascending;
    sorter.Key1 = 11;
    sorter.Sort(cells, CellArea.CreateCellArea(7, 9, 15, 11));

    sorter.Clear();
    sorter.Order1 = SortOrder.Descending;
    sorter.Key1 = 15;
    sorter.Sort(cells, CellArea.CreateCellArea(7, 13, 15, 15));

    sorter.Clear();
    sorter.Order1 = SortOrder.Descending;
    sorter.Key1 = 19;
    sorter.Order2 = SortOrder.Descending;
    sorter.Key2 = 18;
    sorter.Sort(cells, CellArea.CreateCellArea(7, 17, 15, 19));

    sorter.Clear();
    sorter.Order1 = SortOrder.Descending;
    sorter.Key1 = 23;
    sorter.Order2 = SortOrder.Descending;
    sorter.Key2 = 22;
    sorter.Order3 = SortOrder.Descending;
    sorter.Key3 = 21;
    sorter.Sort(cells, CellArea.CreateCellArea(7, 21, 15, 23));

    sorter.Clear();
    sorter.Order1 = SortOrder.Descending;
    sorter.Key1 = 27;
    sorter.Order2 = SortOrder.Ascending;
    sorter.Key2 = 26;
    sorter.Order3 = SortOrder.Descending;
    sorter.Key3 = 25;
    sorter.Sort(cells, CellArea.CreateCellArea(7, 25, 15, 27));
    wb.CalculateFormula();

    Assert.IsTrue(cells[31, 1].BoolValue, "All matched for sorted result");
}
```

### See Also

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


