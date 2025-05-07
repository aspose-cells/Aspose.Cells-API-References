---
title: Chart.NSeries
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets a SeriesCollection collection representing the data series in the chart
type: docs
url: /net/aspose.cells.charts/chart/nseries/
---
## Chart.NSeries property

Gets a [`SeriesCollection`](../../seriescollection/) collection representing the data series in the chart.

```csharp
public SeriesCollection NSeries { get; }
```

### Examples

```csharp
// Called: testAreEqual("=Sheet1!#REF!", chart.NSeries.CategoryData, caseName);
private void Property_NSeries(Workbook workbook)
        {
            Chart chart = workbook.Worksheets["Sheet1"].Charts[0];
            testAreEqual("=Sheet1!$A$1:$A$14", chart.NSeries[0].Values, caseName);
            testAreEqual("=Sheet1!#REF!", chart.NSeries.CategoryData, caseName);

            chart = workbook.Worksheets["Chart1"].Charts[0];
            testAreEqual("=Sheet1!$A$1:$A$14", chart.NSeries[0].Values, caseName);
            testAreEqual("=Sheet1!#REF!", chart.NSeries.CategoryData, caseName);

            chart = workbook.Worksheets["Sheet2"].Charts[0];
            testAreEqual("=Sheet1!$A$1:$A$14", chart.NSeries[0].Values, caseName);
            testAreEqual("=Sheet1!#REF!", chart.NSeries.CategoryData, caseName);
        }
```

### See Also

* class [SeriesCollection](../../seriescollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


