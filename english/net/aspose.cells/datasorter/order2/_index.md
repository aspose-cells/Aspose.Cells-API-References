---
title: DataSorter.Order2
second_title: Aspose.Cells for .NET API Reference
description: DataSorter property. Represents sort order of the second key
type: docs
url: /net/aspose.cells/datasorter/order2/
---
## DataSorter.Order2 property

Represents sort order of the second key.

```csharp
public SortOrder Order2 { get; set; }
```

### Examples

```csharp
// Called: dataSorter.Order2 = SortOrder.Descending;
public void DataSorter_Property_Order2()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    DataSorter dataSorter = workbook.DataSorter;
    dataSorter.Key1 = 1;
    dataSorter.Order1 = SortOrder.Ascending;
    dataSorter.Key2 = 2;
    dataSorter.Order2 = SortOrder.Descending;

    CellArea area = new CellArea();
    {
        area.StartRow = 1;
        area.EndRow = 13;
        area.StartColumn = 1;
        area.EndColumn = 2;
    }
    dataSorter.Sort(workbook.Worksheets[0].Cells, area);
    Assert.AreEqual(workbook.Worksheets[0].Cells["C14"].StringValue, "7435.000");
}
```

### See Also

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


