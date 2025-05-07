---
title: PivotFilter.GetNumberValues
second_title: Aspose.Cells for .NET API Reference
description: PivotFilter method. Gets values of the number filter
type: docs
url: /net/aspose.cells.pivot/pivotfilter/getnumbervalues/
---
## PivotFilter.GetNumberValues method

Gets values of the number filter.

```csharp
public double[] GetNumberValues()
```

### Examples

```csharp
// Called: Assert.AreEqual(2 ,filter.GetNumberValues()[0]);
[Test]
        public void Method_GetNumberValues()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "CellsNet57203.xlsx");
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];
            pt.BaseFields[0].FilterByValue(0, PivotFilterType.ValueLessThan, 2, 0);
            // pt.CalculateData();
            workbook.Save(Constants.PivotTableDestPath + "CellsNet57203.xlsx");
            workbook = new Workbook(Constants.PivotTableDestPath + "CellsNet57203.xlsx");
            pt = workbook.Worksheets[0].PivotTables[0];
            PivotFilter filter = pt.BaseFields[0].GetFilters()[0];
            Assert.AreEqual(PivotFilterType.ValueLessThan,filter.FilterType);//, 
            Assert.AreEqual(2 ,filter.GetNumberValues()[0]);
        }
```

### See Also

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


