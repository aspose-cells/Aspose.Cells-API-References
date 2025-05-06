---
title: Marker.MarkerSizePx
second_title: Aspose.Cells for .NET API Reference
description: Marker property. Represents the marker size in unit of pixels. Applies to line chart scatter chart or radar chart
type: docs
url: /net/aspose.cells.charts/marker/markersizepx/
---
## Marker.MarkerSizePx property

Represents the marker size in unit of pixels. Applies to line chart, scatter chart, or radar chart.

```csharp
public int MarkerSizePx { get; set; }
```

### Examples

```csharp
// Called: series.Marker.MarkerSizePx = 20; // Size in pixels
public static void Property_MarkerSizePx()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            // Obtain the reference of the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to cells
            worksheet.Cells[&quot;A1&quot;].PutValue(50);
            worksheet.Cells[&quot;A2&quot;].PutValue(100);
            worksheet.Cells[&quot;A3&quot;].PutValue(150);
            worksheet.Cells[&quot;B1&quot;].PutValue(60);
            worksheet.Cells[&quot;B2&quot;].PutValue(32);
            worksheet.Cells[&quot;B3&quot;].PutValue(50);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Add NSeries (chart data source) to the chart ranging from &quot;A1&quot; cell to &quot;B3&quot;
            chart.NSeries.Add(&quot;A1:B3&quot;, true);

            // Access the first series
            Series series = chart.NSeries[0];

            // Set marker properties
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.MarkerSize = 10; // Size in points
            series.Marker.MarkerSizePx = 20; // Size in pixels
            series.Marker.ForegroundColor = Color.Red;
            series.Marker.ForegroundColorSetType = FormattingType.Custom;
            series.Marker.BackgroundColor = Color.Yellow;
            series.Marker.BackgroundColorSetType = FormattingType.Custom;

            // Save the workbook
            workbook.Save(&quot;MarkerExample.xlsx&quot;);
        }
```

### See Also

* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


