---
title: "PlotArea.setWidth"
linktitle: "setWidth"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Gets or sets the width of plot-area bounding box in units of 1/4000 of the chart area."
type: docs
weight: 610
url: /nodejs/aspose.cells/plotarea/setwidth/
---

## setWidth()

Gets or sets the width of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X, Y, Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX, InnerY, InnerWidth and InnerHeight properties.For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().
