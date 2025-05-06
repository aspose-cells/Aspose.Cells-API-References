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
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Category&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;A&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;B&quot;);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;C&quot;);
            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Value&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(10);
            worksheet.Cells[&quot;B3&quot;].PutValue(20);
            worksheet.Cells[&quot;B4&quot;].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Add series to the chart
            chart.NSeries.Add(&quot;B2:B4&quot;, true);
            chart.NSeries.CategoryData = &quot;A2:A4&quot;;

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
            font.Name = &quot;Arial&quot;;
            font.Size = 12;
            font.IsBold = true;
            font.Color = Color.Green;

            // Save the workbook
            workbook.Save(&quot;ChartFrameExample.xlsx&quot;);
            workbook.Save(&quot;ChartFrameExample.pdf&quot;);
        }
```

### See Also

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


