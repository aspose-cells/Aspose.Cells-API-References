---
title: PivotField.FilterTop10
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Filters by values of data pivot field
type: docs
url: /net/aspose.cells.pivot/pivotfield/filtertop10/
---
## PivotField.FilterTop10 method

Filters by values of data pivot field.

```csharp
public PivotFilter FilterTop10(int valueFieldIndex, PivotFilterType type, bool isTop, int itemCount)
```

| Parameter | Type | Description |
| --- | --- | --- |
| valueFieldIndex | Int32 | The index of data field in the data region. |
| type | PivotFilterType | The type of filtering data. Only can be Count,Sum and Percent. |
| isTop | Boolean | Indicates whether filter from top or bottom |
| itemCount | Int32 | The item count |

### Examples

```csharp
// Called: pt.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);
public void PivotField_Method_FilterTop10()
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

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


