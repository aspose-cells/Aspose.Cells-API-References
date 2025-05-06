---
title: Series.Type
second_title: Aspose.Cells for .NET API Reference
description: Series property. Gets or sets a data series type
type: docs
url: /net/aspose.cells.charts/series/type/
---
## Series.Type property

Gets or sets a data series' type.

```csharp
public ChartType Type { get; set; }
```

### Examples

```csharp
// Called: series.Type = ChartType.Line;
public static void Property_Type()
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
            worksheet.Cells[&quot;C1&quot;].PutValue(&quot;Q1&quot;);
            worksheet.Cells[&quot;C2&quot;].PutValue(&quot;Q2&quot;);
            worksheet.Cells[&quot;C3&quot;].PutValue(&quot;Y1&quot;);
            worksheet.Cells[&quot;C4&quot;].PutValue(&quot;Y2&quot;);

            // Adding a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            
            // Accessing the instance of the newly added chart
            Chart chart = worksheet.Charts[chartIndex];
            
            // Adding NSeries (chart data source) to the chart ranging from &quot;A1&quot; cell to &quot;B4&quot;
            chart.NSeries.Add(&quot;A1:B4&quot;, true);
            
            // Setting the data source for the category data of NSeries
            chart.NSeries.CategoryData = &quot;C1:C4&quot;;

            // Accessing the SeriesCollection of the chart
            SeriesCollection seriesCollection = chart.NSeries;

            // Setting properties of the SeriesCollection
            seriesCollection.CategoryData = &quot;C1:C4&quot;;
            seriesCollection.SecondCategoryData = &quot;C1:C4&quot;;
            seriesCollection.IsColorVaried = true;

            // Accessing a specific series in the SeriesCollection
            Series series = seriesCollection[0];
            
            // Setting properties of the series
            series.Values = &quot;=B1:B4&quot;;
            series.Name = &quot;First Series&quot;;
            series.Type = ChartType.Line;
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.ForegroundColorSetType = FormattingType.Automatic;
            series.Marker.ForegroundColor = System.Drawing.Color.Black;
            series.Marker.BackgroundColorSetType = FormattingType.Automatic;

            // Saving the Excel file
            workbook.Save(&quot;SeriesCollectionExample.xlsx&quot;);
        }
```

### See Also

* enum [ChartType](../../charttype/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


