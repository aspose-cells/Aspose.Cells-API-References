---
title: PlotArea.InnerWidth
second_title: Aspose.Cells for .NET API Reference
description: PlotArea property. Gets or sets the width of plot area in units of 1/4000 of the chart area
type: docs
url: /net/aspose.cells.charts/plotarea/innerwidth/
---
## PlotArea.InnerWidth property

Gets or sets the width of plot area in units of 1/4000 of the chart area.

```csharp
[Obsolete("Use PlotArea.InnerWidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int InnerWidth { get; set; }
```

### Remarks

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method.

The **X**, **Y**, **Width** and **Height** of **PlotArea** represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** and **InnerHeightRatioToChart** properties.

For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

Note: When InnerWidth is set, the IsInnerMode property will be automatically set to True.

NOTE: This member is now obsolete. Please use PlotArea.InnerWidthRatioToChart property, instead. InnerWidth = InnerWidthRatioToChart * 4000; This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyInnerWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Add chart
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Set chart data
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Configure plot area
            Aspose.Cells.Charts.PlotArea plotArea = chart.PlotArea;
            plotArea.InnerWidth = 2800; // Main demonstration of InnerWidth property
            plotArea.InnerHeight = 1800;
            plotArea.IsInnerMode = true;

            workbook.Save("PlotAreaInnerWidthDemo.xlsx");
        }
    }
}
```

### See Also

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


