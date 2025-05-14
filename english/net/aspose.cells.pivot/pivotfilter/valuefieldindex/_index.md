---
title: PivotFilter.ValueFieldIndex
second_title: Aspose.Cells for .NET API Reference
description: PivotFilter property. Gets the index of value field in the value region
type: docs
url: /net/aspose.cells.pivot/pivotfilter/valuefieldindex/
---
## PivotFilter.ValueFieldIndex property

Gets the index of value field in the value region.

```csharp
public int ValueFieldIndex { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(3,filter.ValueFieldIndex);
public void PivotFilter_Property_ValueFieldIndex()
{
    var wb = new Workbook(Constants.PivotTableSourcePath + "example.xlsm");
    PivotFilter filter = wb.Worksheets[1].PivotTables[0].RowFields[0].GetPivotFilterByType(PivotFilterType.Count);
   Assert.AreEqual(PivotFilterType.Count,filter.FilterType);
    Assert.AreEqual(3,filter.ValueFieldIndex);
    Assert.AreEqual("1",filter.Value1);
    wb = new Workbook(Constants.PivotTableSourcePath + "example.xlsm");
    PivotTable table = wb.Worksheets[1].PivotTables[0];
    table.BaseFields[1].FilterTop10(0, PivotFilterType.Count, true, 1);
    table.BaseFields[1].FilterByLabel(PivotFilterType.CaptionGreaterThan, "1", null);
    Assert.AreEqual(2,table.BaseFields[1].GetFilters().Length);
    table.BaseFields[0].FilterTop10(0, PivotFilterType.Count, true, 10);

    wb.Save(Constants.PivotTableDestPath + "example.xlsx");
    wb = new Workbook(Constants.PivotTableDestPath + "example.xlsx");
    table = wb.Worksheets[1].PivotTables[0];
    Assert.AreEqual(2, table.BaseFields[1].GetFilters().Length);
    Assert.AreEqual(PivotFilterType.Count, table.BaseFields[0].GetFilters()[0].FilterType);

}
```

### See Also

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


