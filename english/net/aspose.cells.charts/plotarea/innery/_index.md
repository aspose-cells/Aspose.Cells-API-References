---
title: PlotArea.InnerY
second_title: Aspose.Cells for .NET API Reference
description: PlotArea property. Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area
type: docs
url: /net/aspose.cells.charts/plotarea/innery/
---
## PlotArea.InnerY property

Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area.

```csharp
[Obsolete("Use PlotArea.InnerYRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int InnerY { get; set; }
```

### Remarks

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method.

The **X**, **Y**, **Width** and **Height** of **PlotArea** represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** and **InnerHeightRatioToChart** properties.

For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

NOTE: This member is now obsolete. Please use PlotArea.InnerYRatioToChart property, instead. InnerY = InnerYRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: plotArea.InnerY = 200;
public static void Property_InnerY()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data
            worksheet.Cells[0, 0].PutValue(&quot;Category&quot;);
            worksheet.Cells[0, 1].PutValue(&quot;Value&quot;);
            worksheet.Cells[1, 0].PutValue(&quot;A&quot;);
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue(&quot;B&quot;);
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue(&quot;C&quot;);
            worksheet.Cells[3, 1].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Set the data range for the chart
            chart.NSeries.Add(&quot;B2:B4&quot;, true);
            chart.NSeries.CategoryData = &quot;A2:A4&quot;;

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
            workbook.Save(&quot;PlotAreaExample.xlsx&quot;);
        }
```

### See Also

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


