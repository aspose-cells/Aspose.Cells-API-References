---
title: PlotArea.InnerYRatioToChart
second_title: Aspose.Cells for .NET API Reference
description: PlotArea property. Gets or gets the x coordinate of the upper top corner of plot area in units of ratio of the chart area
type: docs
url: /net/aspose.cells.charts/plotarea/inneryratiotochart/
---
## PlotArea.InnerYRatioToChart property

Gets or gets the x coordinate of the upper top corner of plot area in units of ratio of the chart area.

```csharp
public double InnerYRatioToChart { get; set; }
```

### Remarks

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method.

The **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** and **HeightRatioToChart** of **PlotArea** represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** and **InnerHeightRatioToChart** properties.

For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

InnerY in Pixel = InnerYRatioToChart * chart.ChartObject.Width. Note: When InnerYRatioToChart is set, the IsInnerMode property will be automatically set to True.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyInnerYRatioToChartDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Set chart data source
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Get the plot area of the chart
            PlotArea plotArea = chart.PlotArea;

            // Display current InnerYRatioToChart value
            Console.WriteLine("Current InnerYRatioToChart value: " + plotArea.InnerYRatioToChart);

            // Change the InnerYRatioToChart value (0.0 to 1.0 represents 0% to 100% of chart area)
            plotArea.InnerYRatioToChart = 0.2;

            // Display the new value
            Console.WriteLine("New InnerYRatioToChart value: " + plotArea.InnerYRatioToChart);

            // Save the workbook
            workbook.Save("PlotAreaPropertyInnerYRatioToChartDemo.xlsx");
        }
    }
}
```

### See Also

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


