---
title: Aspose::Cells::Charts::PlotArea::SetHeight method
linktitle: SetHeight
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::PlotArea::SetHeight method. Gets or sets the height of plot-area bounding box in units of 1/4000 of the chart area in C++.'
type: docs
weight: 1100
url: /cpp/aspose.cells.charts/plotarea/setheight/
---
## PlotArea::SetHeight method


Gets or sets the height of plot-area bounding box in units of 1/4000 of the chart area.


>Deprecated
>
>Use PlotArea.HeightRatioToChart property, instead. 
```cpp
void Aspose::Cells::Charts::PlotArea::SetHeight(int32_t value)
```

## Remarks


The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call [Chart.Calculate()](../../chart/calculate/) method before calling this method. 

The **X**, **Y**, **Width** and **Height** of **[PlotArea](../)** represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** and **InnerHeightRatioToChart** properties.

For excel 2007 or latter, the default value is zero. you should call get the value after calling [Chart.Calculate()](../../chart/calculate/).

Note: When Height is set, the IsInnerMode property will be automatically set to false. 

NOTE: This member is now obsolete. Please use PlotArea.HeightRatioToChart property, instead. Height = HeightRatioToChart * 4000. This property will be removed 12 months later since February 2025. **Aspose** apologizes for any inconvenience you may have experienced.


## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [PlotArea](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
