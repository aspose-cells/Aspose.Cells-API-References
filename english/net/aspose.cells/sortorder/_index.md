---
title: Enum SortOrder
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.SortOrder enum. Represents sort order for the data range
type: docs
url: /net/aspose.cells/sortorder/
---
## SortOrder enumeration

Represents sort order for the data range.

```csharp
public enum SortOrder
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Ascending | `0` | Sorts data in ascending order |
| Descending | `1` | Sorts data in descending order |
| Natural | `2` | Keeps original data order without sorting. Only applies to some special scenarios such as PivotTable. |

### Examples

```csharp
// Called: sorter.Order1 = SortOrder.Descending;
public void Cells_Type_SortOrder()
{
    var workbook = new Workbook(Constants.sourcePath + "example.xlsx");

    var sorter = workbook.DataSorter;

    sorter.Order1 = SortOrder.Descending;
    sorter.Key1 = 0;
    sorter.Order2 = SortOrder.Ascending;
    sorter.Key2 = 1;
    var ca = new CellArea
    {
        StartRow = 0,
        StartColumn = 0,
        EndRow = 20,
        EndColumn = 2
    };
    sorter.Sort(workbook.Worksheets[0].Cells, ca);
    Cells cells = workbook.Worksheets[0].Cells;
    Assert.AreEqual(42005, cells["A4"].DoubleValue);
    Assert.AreEqual("G", cells["B9"].StringValue);
    Assert.AreEqual(41730, cells["A15"].DoubleValue);
    Assert.AreEqual("D", cells["B21"].StringValue);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


