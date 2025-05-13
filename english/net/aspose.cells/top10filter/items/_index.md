---
title: Top10Filter.Items
second_title: Aspose.Cells for .NET API Reference
description: Top10Filter property. Gets and sets the items of the filter
type: docs
url: /net/aspose.cells/top10filter/items/
---
## Top10Filter.Items property

Gets and sets the items of the filter.

```csharp
public int Items { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(2, pivotFilter.GetTop10Value().Items);
public void Top10Filter_Property_Items()
{
    var wb = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    PivotTable pt = wb.Worksheets[0].PivotTables[0];
    pt.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);

    wb.Save(Constants.PivotTableDestPath + "example.xlsx");
    wb = new Workbook(Constants.PivotTableDestPath + "example.xlsx");
    PivotFilter pivotFilter = wb.Worksheets[0].PivotTables[0].BaseFields[0].GetFilters()[0];

    Assert.AreEqual(PivotFilterType.Count, pivotFilter.FilterType);
    Assert.AreEqual(2, pivotFilter.GetTop10Value().Items);
}
```

### See Also

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


