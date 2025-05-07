---
title: PlotArea.InnerX
second_title: Aspose.Cells for .NET API Reference
description: PlotArea property. Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area
type: docs
url: /net/aspose.cells.charts/plotarea/innerx/
---
## PlotArea.InnerX property

Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area.

```csharp
[Obsolete("Use PlotArea.InnerXRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int InnerX { get; set; }
```

### Remarks

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method.

The **X**, **Y**, **Width** and **Height** of **PlotArea** represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** and **InnerHeightRatioToChart** properties.

For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

NOTE: This member is now obsolete. Please use PlotArea.InnerXRatioToChart property, instead. InnerX = InnerXRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: plotArea.InnerX = 200;
public static void Property_InnerX()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Set the data range for the chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

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
            workbook.Save("PlotAreaExample.xlsx");
        }
```

### See Also

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


