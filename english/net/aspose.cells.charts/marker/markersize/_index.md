---
title: Marker.MarkerSize
second_title: Aspose.Cells for .NET API Reference
description: Marker property. Represents the marker size in unit of points. Applies to line chart scatter chart or radar chart
type: docs
url: /net/aspose.cells.charts/marker/markersize/
---
## Marker.MarkerSize property

Represents the marker size in unit of points. Applies to line chart, scatter chart, or radar chart.

```csharp
public int MarkerSize { get; set; }
```

### Examples

```csharp
// Called: series.Marker.MarkerSize = 10; // Size in points
public static void Property_MarkerSize()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            // Obtain the reference of the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to cells
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Add NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
            chart.NSeries.Add("A1:B3", true);

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
            workbook.Save("MarkerExample.xlsx");
        }
```

### See Also

* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


