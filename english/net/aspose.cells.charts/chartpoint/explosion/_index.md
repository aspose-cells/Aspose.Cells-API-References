---
title: ChartPoint.Explosion
second_title: Aspose.Cells for .NET API Reference
description: ChartPoint property. The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter
type: docs
url: /net/aspose.cells.charts/chartpoint/explosion/
---
## ChartPoint.Explosion property

The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter.

```csharp
public int Explosion { get; set; }
```

### Examples

```csharp
// Called: point.Explosion = 15;
public static void Property_Explosion()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Obtaining the reference of the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Adding sample values to cells
            worksheet.Cells[&quot;A1&quot;].PutValue(50);
            worksheet.Cells[&quot;A2&quot;].PutValue(100);
            worksheet.Cells[&quot;A3&quot;].PutValue(150);
            worksheet.Cells[&quot;B1&quot;].PutValue(60);
            worksheet.Cells[&quot;B2&quot;].PutValue(32);
            worksheet.Cells[&quot;B3&quot;].PutValue(50);

            // Adding a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.PieExploded, 5, 0, 25, 10);

            // Accessing the instance of the newly added chart
            Chart chart = worksheet.Charts[chartIndex];

            // Adding NSeries (chart data source) to the chart ranging from &quot;A1&quot; cell to &quot;B3&quot;
            chart.NSeries.Add(&quot;A1:B3&quot;, true);

            // Show Data Labels 
            chart.NSeries[0].DataLabels.ShowValue = true;

            // Accessing the ChartPointCollection
            ChartPointCollection points = chart.NSeries[0].Points;

            // Iterating through the points in the collection
            for (int i = 0; i &lt; points.Count; i++)
            {
                // Get Data Point
                ChartPoint point = points[i];
                
                // Set Pie Explosion
                point.Explosion = 15;
                
                // Set Border Color
                point.Border.Color = System.Drawing.Color.Red;
            }

            // Saving the Excel file
            workbook.Save(&quot;ChartPointCollectionExample.xlsx&quot;);
            workbook.Save(&quot;ChartPointCollectionExample.pdf&quot;);
        }
```

### See Also

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


