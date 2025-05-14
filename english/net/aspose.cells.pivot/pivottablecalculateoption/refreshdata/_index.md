---
title: PivotTableCalculateOption.RefreshData
second_title: Aspose.Cells for .NET API Reference
description: PivotTableCalculateOption property. Indicates whether refreshing data source of the pivottable
type: docs
url: /net/aspose.cells.pivot/pivottablecalculateoption/refreshdata/
---
## PivotTableCalculateOption.RefreshData property

Indicates whether refreshing data source of the pivottable.

```csharp
public bool RefreshData { get; set; }
```

### Examples

```csharp
// Called: option.RefreshData = true;
public void PivotTableCalculateOption_Property_RefreshData()
{
    Workbook w = new Workbook(Constants.PivotTableSourcePath +  "example.xlsx");
    w.Worksheets[0].Cells["B3"].PutValue("a");

    PivotTable pt = w.Worksheets[0].PivotTables[0];
    PivotTableCalculateOption option = new PivotTableCalculateOption();
    option.RefreshData = true;
    pt.CalculateData(option);
   Assert.AreEqual("a",w.Worksheets[0].Cells["E9"].StringValue);
    w.Save(Constants.PivotTableDestPath + "example.xlsx");
}
```

### See Also

* class [PivotTableCalculateOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


