---
title: PlotArea.IsAutomaticSize
second_title: Aspose.Cells for .NET API Reference
description: PlotArea property. Indicates whether the plot area is automatic sized
type: docs
url: /net/aspose.cells.charts/plotarea/isautomaticsize/
---
## PlotArea.IsAutomaticSize property

Indicates whether the plot area is automatic sized.

```csharp
public override bool IsAutomaticSize { get; set; }
```

### Examples

```csharp
// Called: plotArea.IsAutomaticSize = false;
public static void PlotArea_Property_IsAutomaticSize()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Set the data range for the chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Access the plot area of the chart
            PlotArea plotArea = chart.PlotArea;

            // Set properties of the plot area
            plotArea.X = 100;
            plotArea.Y = 100;
            plotArea.Width = 3000;
            plotArea.Height = 2000;
            plotArea.InnerX = 200;
            plotArea.InnerY = 200;
            plotArea.InnerWidth = 2800;
            plotArea.InnerHeight = 1800;
            plotArea.IsAutomaticSize = false;
            plotArea.IsInnerMode = true;
            plotArea.AutoScaleFont = true;
            plotArea.BackgroundMode = BackgroundMode.Transparent;
            plotArea.Shadow = true;

            // Save the workbook
            workbook.Save("PlotAreaExample.xlsx");
        }
```

### See Also

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


