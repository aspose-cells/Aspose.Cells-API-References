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
// Called: PivotFilter pivotFilter = wb.Worksheets[0].PivotTables[0].BaseFields[0].GetFilters()[0];
[Test]
        public void Method_GetFilters()
        {
            var wb = new Workbook(Constants.PivotTableSourcePath + &quot;Net40147.xlsx&quot;);
            PivotTable pt = wb.Worksheets[0].PivotTables[0];
            pt.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);

            wb.Save(Constants.PivotTableDestPath + &quot;Net40147.xlsx&quot;);
            wb = new Workbook(Constants.PivotTableDestPath + &quot;Net40147.xlsx&quot;);
            PivotFilter pivotFilter = wb.Worksheets[0].PivotTables[0].BaseFields[0].GetFilters()[0];

            Assert.AreEqual(PivotFilterType.Count, pivotFilter.FilterType);
            Assert.AreEqual(2, pivotFilter.GetTop10Value().Items);
        }
```

### See Also

* class [PivotFilter](../../pivotfilter/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


