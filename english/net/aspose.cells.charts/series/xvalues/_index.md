---
title: Series.XValues
second_title: Aspose.Cells for .NET API Reference
description: Series property. Represents the x values of the chart series
type: docs
url: /net/aspose.cells.charts/series/xvalues/
---
## Series.XValues property

Represents the x values of the chart series.

```csharp
public string XValues { get; set; }
```

### Examples

```csharp
// Called: series.XValues = "{1,2,3,4,5}";
public void Series_Property_XValues()
{
    int nSeries = 2;
    var workbook = new Workbook();
    int index = workbook.Worksheets.Add();
    var worksheet = workbook.Worksheets[index];
    index = worksheet.Charts.Add(ChartType.Scatter, 0, 0, 5, 2);
    var chart = worksheet.Charts[index];

    chart.ChartObject.HeightInch = 4;
    chart.ChartObject.WidthInch = 6;

    string[] yvalues = { "{1,3,5,7,9}", "{2,4,6,8,10}" };

    for (int i = 0; i < nSeries; ++i)
    {
        index = chart.NSeries.Add("A1", false);
        var series = chart.NSeries[index];
        series.XValues = "{1,2,3,4,5}";
        series.Values = yvalues[i];
        index = series.TrendLines.Add(TrendlineType.Linear);
    }

    var entries = chart.Legend.LegendEntries;
    entries[0].IsDeleted = true;

    //  workbook.Save(@"Test3.pdf");
    workbook.Save(Constants.destPath + @"example.xlsx");
}
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


