---
title: Series.TrendLines
second_title: Aspose.Cells for .NET API Reference
description: Series property. Returns all the trendlines of this series
type: docs
url: /net/aspose.cells.charts/series/trendlines/
---
## Series.TrendLines property

Returns all the trendlines of this series.

```csharp
public TrendlineCollection TrendLines { get; }
```

### Examples

```csharp
// Called: int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, &amp;quot;MyTrendLine&amp;quot;);
public static void Property_TrendLines()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            
            // Adding a new worksheet to the Excel object
            int sheetIndex = workbook.Worksheets.Add();
            
            // Obtaining the reference of the newly added worksheet by passing its sheet index
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Adding sample values to cells
            worksheet.Cells[&quot;A1&quot;].PutValue(50);
            worksheet.Cells[&quot;A2&quot;].PutValue(100);
            worksheet.Cells[&quot;A3&quot;].PutValue(150);
            worksheet.Cells[&quot;A4&quot;].PutValue(200);
            worksheet.Cells[&quot;B1&quot;].PutValue(60);
            worksheet.Cells[&quot;B2&quot;].PutValue(32);
            worksheet.Cells[&quot;B3&quot;].PutValue(50);
            worksheet.Cells[&quot;B4&quot;].PutValue(40);

            // Adding a chart to the worksheet
            int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 3, 3, 15, 10);
            Chart chart = workbook.Worksheets[0].Charts[chartIndex];
            
            // Adding NSeries (chart data source) to the chart ranging from &quot;A1&quot; cell to &quot;B4&quot;
            chart.NSeries.Add(&quot;A1:A4&quot;, true);
            chart.NSeries.Add(&quot;B1:B4&quot;, true);
            
            // Adding a trendline to the first series
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, &quot;MyTrendLine&quot;);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Setting trendline properties
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = true;
            trendline.Color = Color.Red;

            // Saving the Excel file
            workbook.Save(&quot;TrendlineCollectionExample.xlsx&quot;);
        }
```

### See Also

* class [TrendlineCollection](../../trendlinecollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


