---
title: PlotArea.HeightRatioToChart
second_title: Aspose.Cells for .NET API Reference
description: PlotArea property. Gets or sets the height of plotarea bounding box in units of ratio of the chart area
type: docs
url: /net/aspose.cells.charts/plotarea/heightratiotochart/
---
## PlotArea.HeightRatioToChart property

Gets or sets the height of plot-area bounding box in units of ratio of the chart area.

```csharp
public override double HeightRatioToChart { get; set; }
```

### Remarks

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method.

The **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** and **HeightRatioToChart** of **PlotArea** represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** and **InnerHeightRatioToChart** properties.

For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

HeightPixel = HeightRatioToChart * chart.ChartObject.Width.

### See Also

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


