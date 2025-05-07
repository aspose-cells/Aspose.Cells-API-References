---
title: ChartFrame.IsInnerMode
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. Indicates whether the size of the plot area size includes the tick marks and the axis labels. False specifies that the size shall determine the size of the plot area the tick marks and the axis labels
type: docs
url: /net/aspose.cells.charts/chartframe/isinnermode/
---
## ChartFrame.IsInnerMode property

Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels.

```csharp
public bool IsInnerMode { get; set; }
```

### Remarks

Only for Xlsx file.

### Examples

```csharp
// Called: chartFrame.IsInnerMode = false;
public static void Property_IsInnerMode()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Add series to the chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Access the chart frame
            ChartFrame chartFrame = chart.ChartArea;

            // Set properties of the chart frame
            chartFrame.IsInnerMode = false;
            chartFrame.AutoScaleFont = true;
            chartFrame.BackgroundMode = BackgroundMode.Transparent;
            chartFrame.IsAutomaticSize = true;
            chartFrame.X = 1000; // 1/4000 of the chart area
            chartFrame.Y = 1000; // 1/4000 of the chart area
            chartFrame.Width = 3000; // 1/4000 of the chart area
            chartFrame.Height = 2000; // 1/4000 of the chart area
            chartFrame.Shadow = true;

            // Access and modify the border of the chart frame
            Line border = chartFrame.Border;
            border.Color = Color.Red;
            border.Style = LineType.Solid;

            // Access and modify the area of the chart frame
            Area area = chartFrame.Area;
            area.ForegroundColor = Color.Yellow;
            area.BackgroundColor = Color.Blue;

            // Access and modify the font of the chart frame
            Aspose.Cells.Font font = chartFrame.TextFont;
            font.Name = "Arial";
            font.Size = 12;
            font.IsBold = true;
            font.Color = Color.Green;

            // Save the workbook
            workbook.Save("ChartFrameExample.xlsx");
            workbook.Save("ChartFrameExample.pdf");
        }
```

### See Also

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


