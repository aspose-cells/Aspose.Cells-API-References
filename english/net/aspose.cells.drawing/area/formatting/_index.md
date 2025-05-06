---
title: Area.Formatting
second_title: Aspose.Cells for .NET API Reference
description: Area property. Represents the formatting of the area
type: docs
url: /net/aspose.cells.drawing/area/formatting/
---
## Area.Formatting property

Represents the formatting of the area.

```csharp
public FormattingType Formatting { get; set; }
```

### Examples

```csharp
// Called: chart.NSeries[0].Area.Formatting = FormattingType.None;
public static void Property_Formatting()
        {
            // Instantiate a Workbook object
            Workbook workbook = new Workbook();
            
            // Adding a new worksheet to the Workbook object
            int sheetIndex = workbook.Worksheets.Add();
            
            // Obtaining the reference of the newly added worksheet by passing its sheet index
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Adding sample values to cells
            worksheet.Cells[&quot;A1&quot;].PutValue(50);
            worksheet.Cells[&quot;A2&quot;].PutValue(100);
            worksheet.Cells[&quot;A3&quot;].PutValue(150);
            worksheet.Cells[&quot;B1&quot;].PutValue(60);
            worksheet.Cells[&quot;B2&quot;].PutValue(32);
            worksheet.Cells[&quot;B3&quot;].PutValue(50);
            
            // Adding a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            
            // Accessing the instance of the newly added chart
            Chart chart = worksheet.Charts[chartIndex];
            
            // Adding NSeries (chart data source) to the chart ranging from &quot;A1&quot; cell to &quot;B3&quot;
            chart.NSeries.Add(&quot;A1:B3&quot;, true);
            
            // Setting the foreground color of the plot area
            chart.PlotArea.Area.ForegroundColor = Color.Blue;
            chart.PlotArea.Area.Formatting = FormattingType.Custom;
            
            // Setting the foreground color of the chart area
            chart.ChartArea.Area.ForegroundColor = Color.Yellow;
            chart.ChartArea.Area.Formatting = FormattingType.Automatic;
            
            // Setting the foreground color of the 1st NSeries area
            chart.NSeries[0].Area.ForegroundColor = Color.Red;
            chart.NSeries[0].Area.Formatting = FormattingType.None;
            
            // Setting the foreground color of the area of the 1st NSeries point
            chart.NSeries[0].Points[0].Area.ForegroundColor = Color.Cyan;
            chart.NSeries[0].Points[0].Area.Formatting = FormattingType.Custom;
            
            // Saving the Excel file
            workbook.Save(&quot;FormattingTypeExample.xlsx&quot;);
            workbook.Save(&quot;FormattingTypeExample.pdf&quot;);
        }
```

### See Also

* enum [FormattingType](../../../aspose.cells.charts/formattingtype/)
* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


