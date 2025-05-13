---
title: DataSorter.Order1
second_title: Aspose.Cells for .NET API Reference
description: DataSorter property. Represents sort order of the first key
type: docs
url: /net/aspose.cells/datasorter/order1/
---
## DataSorter.Order1 property

Represents sort order of the first key.

```csharp
public SortOrder Order1 { get; set; }
```

### Examples

```csharp
// Called: wb.DataSorter.Order1 = SortOrder.Ascending;
public void DataSorter_Property_Order1()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");

    wb.CalculateFormula();

    wb.DataSorter.Order1 = SortOrder.Ascending;
    wb.DataSorter.SortLeftToRight = true;

    Worksheet ws = wb.Worksheets["Output"];

    CellArea ca = CellArea.CreateCellArea("T1", "AK5000");

    wb.DataSorter.Key1 = 12;
    wb.DataSorter.Sort(ws.Cells, ca);
    Assert.AreEqual(ws.Cells["Y1"].Formula, "=Y4");
    wb.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


