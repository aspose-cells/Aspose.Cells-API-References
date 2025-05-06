---
title: Marker.ForegroundColor
second_title: Aspose.Cells for .NET API Reference
description: Marker property. Represents the marker foreground color in a line chart scatter chart or radar chart
type: docs
url: /net/aspose.cells.charts/marker/foregroundcolor/
---
## Marker.ForegroundColor property

Represents the marker foreground color in a line chart, scatter chart, or radar chart.

```csharp
public Color ForegroundColor { get; set; }
```

### Examples

```csharp
// Called: marker.ForegroundColor = Color.Red;
public static void Property_ForegroundColor()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the chart
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Category&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;A&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;B&quot;);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;C&quot;);

            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Value&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(10);
            worksheet.Cells[&quot;B3&quot;].PutValue(20);
            worksheet.Cells[&quot;B4&quot;].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Add the data series to the chart
            chart.NSeries.Add(&quot;B2:B4&quot;, true);
            chart.NSeries.CategoryData = &quot;A2:A4&quot;;

            // Access the marker of the first series
            Marker marker = chart.NSeries[0].Marker;

            // Set the marker style
            marker.MarkerStyle = ChartMarkerType.Circle;

            // Set the marker size
            marker.MarkerSize = 10;

            // Set the marker foreground and background colors
            marker.ForegroundColor = Color.Red;
            marker.BackgroundColor = Color.Yellow;

            // Save the workbook
            workbook.Save(&quot;ChartMarkerTypeExample.xlsx&quot;);
            workbook.Save(&quot;ChartMarkerTypeExample.pdf&quot;);
            return;
        }
```

### See Also

* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


