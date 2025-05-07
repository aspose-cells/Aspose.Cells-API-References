---
title: Series.TrendLines
second_title: Aspose.Cells for .NET API Reference
description: Series property. Returns all the trendlines of this series
type: docs
url: /net/aspose.cells.charts/series/trendlines/
---
## Series.TrendLines property

Returns all the trendlines of this series.

```csharp
public TrendlineCollection TrendLines { get; }
```

### Examples

```csharp
// Called: Trendline trendline = chart.NSeries[seriesIndex].TrendLines[index];
private static void Property_TrendLines(Chart chart, int seriesIndex, TrendlineType trendlineType, string trendlineName)
        {
            // Adding a trendline of the specified type to the specified series
            int index = chart.NSeries[seriesIndex].TrendLines.Add(trendlineType);
            Trendline trendline = chart.NSeries[seriesIndex].TrendLines[index];
            
            // Setting the custom name of the trendline
            trendline.Name = trendlineName;
            
            // Displaying the equation on the chart
            trendline.DisplayEquation = true;
            
            // Displaying the R-Squared value on the chart
            trendline.DisplayRSquared = true;
            
            // Setting the color of the trendline
            trendline.Color = Color.Red;
        }
```

### See Also

* class [TrendlineCollection](../../trendlinecollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


