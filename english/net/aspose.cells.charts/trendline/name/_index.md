---
title: Trendline.Name
second_title: Aspose.Cells for .NET API Reference
description: Trendline property. Returns the name of the trendline
type: docs
url: /net/aspose.cells.charts/trendline/name/
---
## Trendline.Name property

Returns the name of the trendline.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: trendline.Name = trendlineName;
private static void Trendline_Property_Name(Chart chart, int seriesIndex, TrendlineType trendlineType, string trendlineName)
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

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


