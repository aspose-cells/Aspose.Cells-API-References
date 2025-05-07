---
title: Marker.BackgroundColor
second_title: Aspose.Cells for .NET API Reference
description: Marker property. Represents the marker background color in a line chart scatter chart or radar chart
type: docs
url: /net/aspose.cells.charts/marker/backgroundcolor/
---
## Marker.BackgroundColor property

Represents the marker background color in a line chart, scatter chart, or radar chart.

```csharp
public Color BackgroundColor { get; set; }
```

### Examples

```csharp
// Called: marker.BackgroundColor = Color.Yellow;
public static void Property_BackgroundColor()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Add the data series to the chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

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
            workbook.Save("ChartMarkerTypeExample.xlsx");
            workbook.Save("ChartMarkerTypeExample.pdf");
            return;
        }
```

### See Also

* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


