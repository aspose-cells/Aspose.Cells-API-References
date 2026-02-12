---
title: Aspose::Cells::Charts::PlotArea::SetInnerHeightRatioToChart method
linktitle: SetInnerHeightRatioToChart
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::PlotArea::SetInnerHeightRatioToChart method. Gets or sets the height of plot area in units of ratio of the chart area in C++.'
type: docs
weight: 3500
url: /cpp/aspose.cells.charts/plotarea/setinnerheightratiotochart/
---
## PlotArea::SetInnerHeightRatioToChart method


Gets or sets the height of plot area in units of ratio of the chart area.

```cpp
void Aspose::Cells::Charts::PlotArea::SetInnerHeightRatioToChart(double value)
```

## Remarks


The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call [Chart.Calculate()](../../chart/calculate/) method before calling this method. 

The **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** and **HeightRatioToChart** of **[PlotArea](../)** represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** and **InnerHeightRatioToChart** properties.

For excel 2007 or latter, the default value is zero. you should call get the value after calling [Chart.Calculate()](../../chart/calculate/).

InnerHeight in Pixel = InnerXRatioToChart * chart.ChartObject.Width. Note: When InnerHeightRatioToChart is set, the IsInnerMode property will be automatically set to True. 
## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [PlotArea](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
