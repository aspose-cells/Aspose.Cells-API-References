---
title: PivotFilter.GetTop10Value
second_title: Aspose.Cells for .NET API Reference
description: PivotFilter method. Gets top 10 setting of the filter
type: docs
url: /net/aspose.cells.pivot/pivotfilter/gettop10value/
---
## PivotFilter.GetTop10Value method

Gets top 10 setting of the filter.

```csharp
public Top10Filter GetTop10Value()
```

### Examples

```csharp
// Called: Assert.AreEqual(2, pivotFilter.GetTop10Value().Items);
[Test]
        public void Method_GetTop10Value()
        {
            var wb = new Workbook(Constants.PivotTableSourcePath + "Net40147.xlsx");
            PivotTable pt = wb.Worksheets[0].PivotTables[0];
            pt.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);

            wb.Save(Constants.PivotTableDestPath + "Net40147.xlsx");
            wb = new Workbook(Constants.PivotTableDestPath + "Net40147.xlsx");
            PivotFilter pivotFilter = wb.Worksheets[0].PivotTables[0].BaseFields[0].GetFilters()[0];

            Assert.AreEqual(PivotFilterType.Count, pivotFilter.FilterType);
            Assert.AreEqual(2, pivotFilter.GetTop10Value().Items);
        }
```

### See Also

* class [Top10Filter](../../../aspose.cells/top10filter/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


