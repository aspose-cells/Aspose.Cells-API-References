---
title: PlotArea.YRatioToChart
second_title: Aspose.Cells for .NET API Reference
description: PlotArea property. Gets or gets the y coordinate of the upper top corner of plotarea bounding box in units of ratio of the chart area
type: docs
url: /net/aspose.cells.charts/plotarea/yratiotochart/
---
## PlotArea.YRatioToChart property

Gets or gets the y coordinate of the upper top corner of plot-area bounding box in units of ratio of the chart area.

```csharp
public override double YRatioToChart { get; set; }
```

### Remarks

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method.

The **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** and **HeightRatioToChart** of **PlotArea** represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** and **InnerHeightRatioToChart** properties.

For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

YPixel = YRatioToChart * chart.ChartObject.Width. Note: When YRatioToChart is set, the IsInnerMode property will be automatically set to false.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyYRatioToChartDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Get the plot area of the chart
            PlotArea plotArea = chart.PlotArea;

            // Display the current YRatioToChart value
            Console.WriteLine("Current YRatioToChart value: " + plotArea.YRatioToChart);

            // Set a new YRatioToChart value (0.1 means 10% from the top of the chart area)
            plotArea.YRatioToChart = 0.1;

            // Display the new YRatioToChart value
            Console.WriteLine("New YRatioToChart value: " + plotArea.YRatioToChart);

            // Save the workbook to see the effect
            workbook.Save("PlotAreaYRatioToChartDemo.xlsx");
        }
    }
}
```

### See Also

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


