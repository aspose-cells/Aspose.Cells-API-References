---
title: PivotField.GetFilters
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Gets all pivot filters of this pivot field
type: docs
url: /net/aspose.cells.pivot/pivotfield/getfilters/
---
## PivotField.GetFilters method

Gets all pivot filters of this pivot field.

```csharp
public PivotFilter[] GetFilters()
```

### Examples

```csharp
// Called: Assert.AreEqual(1, pt.BaseFields[1].GetFilters().Length);
public void PivotField_Method_GetFilters()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    PivotTable pt = workbook.Worksheets[0].PivotTables[0];
    pt.BaseFields[1].FilterByDate(PivotFilterType.DateBetween, DateTime.Now, DateTime.Now.AddDays(1));
    workbook.Save(Constants.PivotTableDestPath + "example.xlsx");
    workbook = new Workbook(Constants.PivotTableDestPath + "example.xlsx");
    pt = workbook.Worksheets[0].PivotTables[0];
    Assert.AreEqual(1, pt.BaseFields[1].GetFilters().Length);
    PivotFilter filter = pt.BaseFields[1].GetFilters()[0];
    Assert.AreEqual(PivotFilterType.DateBetween, filter.FilterType);
    Assert.AreEqual(DateTime.Now.Day, filter.GetDateTimeValues()[0].Day);
    Assert.AreEqual(DateTime.Now.AddDays(1).Day, filter.GetDateTimeValues()[1].Day);
}
```

### See Also

* class [PivotFilter](../../pivotfilter/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


