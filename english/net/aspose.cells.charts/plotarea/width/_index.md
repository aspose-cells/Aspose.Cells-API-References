---
title: PlotArea.Width
second_title: Aspose.Cells for .NET API Reference
description: PlotArea property. Gets or sets the width of plotarea bounding box in units of 1/4000 of the chart area
type: docs
url: /net/aspose.cells.charts/plotarea/width/
---
## PlotArea.Width property

Gets or sets the width of plot-area bounding box in units of 1/4000 of the chart area.

```csharp
[Obsolete("Use PlotArea.WidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Width { get; set; }
```

### Remarks

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method.

The **X**, **Y**, **Width** and **Height** of **PlotArea** represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** and **InnerHeightRatioToChart** properties.

For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

Note: When Width is set, the IsInnerMode property will be automatically set to false.

NOTE: This member is now obsolete. Please use PlotArea.WidthRatioToChart property, instead. Width = WidthRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyWidthDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Add a column chart
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Set chart data range
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Access and modify plot area properties
            PlotArea plotArea = chart.PlotArea;
            plotArea.Width = 3000; // Demonstrating Width property usage
            plotArea.Height = 2000;

            // Save the workbook
            workbook.Save("PlotAreaWidthDemo.xlsx");
        }
    }
}
```

### See Also

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


