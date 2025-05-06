---
title: Trendline.DisplayRSquared
second_title: Aspose.Cells for .NET API Reference
description: Trendline property. Represents if the Rsquared value of the trendline is displayed on the chart in the same data label as the equation. Setting this property to True automatically turns on data labels
type: docs
url: /net/aspose.cells.charts/trendline/displayrsquared/
---
## Trendline.DisplayRSquared property

Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). Setting this property to True automatically turns on data labels.

```csharp
public bool DisplayRSquared { get; set; }
```

### Examples

```csharp
// Called: trendline.DisplayRSquared = true;
private static void Property_DisplayRSquared(Chart chart, int seriesIndex, TrendlineType trendlineType, string trendlineName)
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


