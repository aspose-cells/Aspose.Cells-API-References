---
title: PivotFilter.UseWholeDay
second_title: Aspose.Cells for .NET API Reference
description: PivotFilter property. Indicates whether uses whole days in its filtering criteria
type: docs
url: /net/aspose.cells.pivot/pivotfilter/usewholeday/
---
## PivotFilter.UseWholeDay property

Indicates whether uses whole days in its filtering criteria.

```csharp
public bool UseWholeDay { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(pt.BaseFields[1].GetFilters()[0].UseWholeDay);
public void PivotFilter_Property_UseWholeDay()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    PivotTable pt = workbook.Worksheets[0].PivotTables[0];
    Assert.IsTrue(pt.BaseFields[1].GetFilters()[0].UseWholeDay);
    workbook.Save(Constants.PivotTableDestPath + "example.xlsb");
        
    workbook = new Workbook(Constants.PivotTableDestPath + "example.xlsb");
    pt = workbook.Worksheets[0].PivotTables[0];
    Assert.IsTrue(pt.BaseFields[1].GetFilters()[0].UseWholeDay);
    workbook.Save(Constants.PivotTableDestPath + "example.xlsx");
    workbook = new Workbook(Constants.PivotTableDestPath + "example.xlsx");
    pt = workbook.Worksheets[0].PivotTables[0];
    Assert.IsTrue(pt.BaseFields[1].GetFilters()[0].UseWholeDay);
}
```

### See Also

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


