---
title: Aspose::Cells::Charts::PlotArea::SetInnerWidthRatioToChart method
linktitle: SetInnerWidthRatioToChart
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::PlotArea::SetInnerWidthRatioToChart method. Gets or sets the width of plot area in units of ratio of the chart area in C++.'
type: docs
weight: 3700
url: /cpp/aspose.cells.charts/plotarea/setinnerwidthratiotochart/
---
## PlotArea::SetInnerWidthRatioToChart method


Gets or sets the width of plot area in units of ratio of the chart area.

```cpp
void Aspose::Cells::Charts::PlotArea::SetInnerWidthRatioToChart(double value)
```

## Remarks


The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call [Chart.Calculate()](../../chart/calculate/) method before calling this method. 

The **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** and **HeightRatioToChart** of **[PlotArea](../)** represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** and **InnerHeightRatioToChart** properties.

For excel 2007 or latter, the default value is zero. you should call get the value after calling [Chart.Calculate()](../../chart/calculate/).

InnerWidth in Pixel = InnerXRatioToChart * chart.ChartObject.Width. Note: When InnerWidthRatioToChart is set, the IsInnerMode property will be automatically set to True. 
## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [PlotArea](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
