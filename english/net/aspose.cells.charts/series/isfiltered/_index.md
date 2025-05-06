---
title: Series.IsFiltered
second_title: Aspose.Cells for .NET API Reference
description: Series property. Indicates whether the series is selected or filtered.True represents this series is filtered and it will not be displayed on the chart
type: docs
url: /net/aspose.cells.charts/series/isfiltered/
---
## Series.IsFiltered property

Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be displayed on the chart.

```csharp
public bool IsFiltered { get; set; }
```

### Examples

```csharp
// Called: nSeries[1].IsFiltered = true;
[Test]
        public void Property_IsFiltered()
        {
            //Test for FilteredNSeries and series IsFiltered 
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;SeriesFiltered.xlsx&quot;);
            ChartCollection charts = workbook.Worksheets[0].Charts;
            Chart chart = charts[&quot;Chart 1&quot;];
            SeriesCollection nSeriesFiltered = chart.FilteredNSeries;
            Assert.AreEqual(2, nSeriesFiltered.Count);
            SeriesCollection nSeries = chart.NSeries;
            Assert.AreEqual(4, nSeries.Count);
            //When nSeries[1].IsFiltered = true, the series nSeries[1] will be removed from the selected series list,and the second series(nSeries[2]) 
            //will move forward one and become the first one(Series[1]),which can be quite confusing. Therefore, we delete from the end to the beginning.
            nSeries[1].IsFiltered = true;
            nSeries[0].IsFiltered = true;
            Assert.AreEqual(2, chart.NSeries.Count);//from 4 to 2
            Assert.AreEqual(4, chart.FilteredNSeries.Count);//from 2 to 4
            workbook.Save(Constants.destPath + &quot;SeriesFiltered-out.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;SeriesFiltered-out.xlsx&quot;);
            Chart chart1 = workbook.Worksheets[0].Charts[&quot;Chart 1&quot;];
            //checking after save
            Assert.AreEqual(2, chart.NSeries.Count);
            Assert.AreEqual(4, chart.FilteredNSeries.Count);
        }
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


