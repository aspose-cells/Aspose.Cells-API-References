---
title: ChartPoint.XValue
second_title: Aspose.Cells for .NET API Reference
description: ChartPoint property. Gets or sets the X value of the chart point
type: docs
url: /net/aspose.cells.charts/chartpoint/xvalue/
---
## ChartPoint.XValue property

Gets or sets the X value of the chart point.

```csharp
public object XValue { get; set; }
```

### Examples

```csharp
// Called: point.XValue = &amp;quot;Category &amp;quot; + (i + 1);
public static void Property_XValue()
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

            // Iterate through each point in the series
            for (int i = 0; i &lt; chart.NSeries[0].Points.Count; i++)
            {
                // Get Data Point
                ChartPoint point = chart.NSeries[0].Points[i];

                // Set Pie Explosion
                point.Explosion = 15;

                // Set Border Color
                point.Border.Color = Color.Red;

                // Set Shadow
                point.Shadow = true;

                // Set YValue
                point.YValue = 100 + i * 10;

                // Set XValue
                point.XValue = &quot;Category &quot; + (i + 1);

                // Set IsInSecondaryPlot
                point.IsInSecondaryPlot = false;
            }

            // Saving the Excel file
            workbook.Save(&quot;ChartPointExample.xlsx&quot;);
            workbook.Save(&quot;ChartPointExample.pdf&quot;);
        }
```

### See Also

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


