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

NOTE: This member is now obsolete. Please use PlotArea.InnerWidthRatioToChart property, instead. InnerWidth = InnerWidthRatioToChart * 4000; This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


