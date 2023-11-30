﻿---
title: Aspose::Cells::Charts::PlotArea::GetY method
linktitle: GetY
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::PlotArea::GetY method. Gets or gets the y coordinate of the upper top corner of plot-area bounding box in units of 1/4000 of the chart area in C++.'
type: docs
weight: 800
url: /cpp/aspose.cells.charts/plotarea/gety/
---
## PlotArea::GetY method


Gets or gets the y coordinate of the upper top corner of plot-area bounding box in units of 1/4000 of the chart area.

```cpp
int32_t Aspose::Cells::Charts::PlotArea::GetY()
```

## Remarks


The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call [Chart.Calculate()](../../chart/calculate/) method before calling this method. 

The **X**, **Y**, **Width** and **Height** of **[PlotArea](../)** represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call **InnerX**, **InnerY**, **InnerWidth** and **InnerHeight** properties.

For excel 2007 or latter, the default value is zero. you should call get the value after calling [Chart.Calculate()](../../chart/calculate/).
## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [PlotArea](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
