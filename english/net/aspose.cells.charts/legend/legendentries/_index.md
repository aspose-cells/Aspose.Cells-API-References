---
title: Legend.LegendEntries
second_title: Aspose.Cells for .NET API Reference
description: Legend property. Gets a collection of all the LegendEntry objects in the specified chart legend. Setting the legend entries of the surface chart is not supported. So it will return null if the chart type is surface chart type
type: docs
url: /net/aspose.cells.charts/legend/legendentries/
---
## Legend.LegendEntries property

Gets a collection of all the LegendEntry objects in the specified chart legend. Setting the legend entries of the surface chart is not supported. So it will return null if the chart type is surface chart type.

```csharp
public LegendEntryCollection LegendEntries { get; }
```

### Examples

```csharp
// Called: var entries = chart.Legend.LegendEntries;
[Test]
        public void Property_LegendEntries()
        {
            int nSeries = 2;
            var workbook = new Workbook();
            int index = workbook.Worksheets.Add();
            var worksheet = workbook.Worksheets[index];
            index = worksheet.Charts.Add(ChartType.Scatter, 0, 0, 5, 2);
            var chart = worksheet.Charts[index];

            chart.ChartObject.HeightInch = 4;
            chart.ChartObject.WidthInch = 6;

            string[] yvalues = { &quot;{1,3,5,7,9}&quot;, &quot;{2,4,6,8,10}&quot; };

            for (int i = 0; i &lt; nSeries; ++i)
            {
                index = chart.NSeries.Add(&quot;A1&quot;, false);
                var series = chart.NSeries[index];
                series.XValues = &quot;{1,2,3,4,5}&quot;;
                series.Values = yvalues[i];
                index = series.TrendLines.Add(TrendlineType.Linear);
            }

            var entries = chart.Legend.LegendEntries;

            workbook.Save(Constants.destPath + @&quot;CELLSNET47506.pdf&quot;);
            workbook.Save(Constants.destPath + @&quot;CELLSNET47506.xlsx&quot;);
        }
```

### See Also

* class [LegendEntryCollection](../../legendentrycollection/)
* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


