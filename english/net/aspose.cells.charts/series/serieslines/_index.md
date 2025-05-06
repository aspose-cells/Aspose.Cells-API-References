---
title: Series.SeriesLines
second_title: Aspose.Cells for .NET API Reference
description: Series property. Returns a SeriesLines object that represents the series lines for a stacked bar chart or a stacked column chart. Applies only to stacked bar and stacked column charts
type: docs
url: /net/aspose.cells.charts/series/serieslines/
---
## Series.SeriesLines property

Returns a SeriesLines object that represents the series lines for a stacked bar chart or a stacked column chart. Applies only to stacked bar and stacked column charts.

```csharp
public Line SeriesLines { get; }
```

### Examples

```csharp
// Called: chart.NSeries[1].SeriesLines.FormattingType = ChartLineFormattingType.Gradient;
public static void Property_SeriesLines()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Add a new worksheet to the workbook
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
            
            // Add series to the chart
            chart.NSeries.Add(&quot;A1:B3&quot;, true);
            
            // Set the category data
            chart.NSeries.CategoryData = &quot;A1:A3&quot;;
            
            // Set different line formatting types for the series
            chart.NSeries[0].SeriesLines.FormattingType = ChartLineFormattingType.Solid;
            chart.NSeries[0].SeriesLines.Color = Color.Red;
            
            // Add another series with different formatting
            chart.NSeries.Add(&quot;B1:B3&quot;, true);
            chart.NSeries[1].SeriesLines.FormattingType = ChartLineFormattingType.Gradient;
            chart.NSeries[1].SeriesLines.Color = Color.Blue;
            
            // Save the workbook
            workbook.Save(&quot;ChartLineFormattingTypeExample.xlsx&quot;);
            workbook.Save(&quot;ChartLineFormattingTypeExample.pdf&quot;);
        }
```

### See Also

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


