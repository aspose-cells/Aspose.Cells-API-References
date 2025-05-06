---
title: ChartFrame.BackgroundMode
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. Gets and sets the display mode of the background
type: docs
url: /net/aspose.cells.charts/chartframe/backgroundmode/
---
## ChartFrame.BackgroundMode property

Gets and sets the display mode of the background

```csharp
public BackgroundMode BackgroundMode { get; set; }
```

### Examples

```csharp
// Called: chartArea.BackgroundMode = BackgroundMode.Opaque;
public static void Property_BackgroundMode()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Obtain the reference of the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add some sample data to cells
            worksheet.Cells[&quot;A1&quot;].PutValue(50);
            worksheet.Cells[&quot;A2&quot;].PutValue(100);
            worksheet.Cells[&quot;A3&quot;].PutValue(150);
            worksheet.Cells[&quot;B1&quot;].PutValue(60);
            worksheet.Cells[&quot;B2&quot;].PutValue(32);
            worksheet.Cells[&quot;B3&quot;].PutValue(50);
            
            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Add NSeries (chart data source) to the chart ranging from &quot;A1&quot; cell to &quot;B3&quot;
            chart.NSeries.Add(&quot;A1:B3&quot;, true);
            
            // Access the chart area
            ChartArea chartArea = chart.ChartArea;

            // Set the foreground color of the chart area
            chartArea.Area.ForegroundColor = Color.Yellow;

            // Set the background mode of the chart area
            chartArea.BackgroundMode = BackgroundMode.Opaque;
            chartArea.Area.Transparency = 0.8;           
            
            
            // Set the shadow of the chart area
            chartArea.Shadow = true;
            
            // Save the workbook
            workbook.Save(&quot;BackgroundModeExample.xlsx&quot;);
            workbook.Save(&quot;BackgroundModeExample.pdf&quot;);
        }
```

### See Also

* enum [BackgroundMode](../../backgroundmode/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


