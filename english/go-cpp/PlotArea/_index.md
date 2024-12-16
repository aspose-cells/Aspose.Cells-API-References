---
title: PlotArea Class 
linktitle: PlotArea
second_title: Aspose.Cells for Go via C++ API Reference
description: 'PlotArea class. Encapsulates the object that represents plotarea in Go.'
type: docs
weight: 200
url: /go-cpp/plotarea/
---

## PlotArea class

Encapsulates the object that represents the plot area in a chart.

```go

type PlotArea struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
|[NewPlotArea](./newplotarea/) | Constructs from a parent object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetX](./getx/) | Gets or gets the x coordinate of the upper left corner of plot-area bounding box in units of 1/4000 of the chart area. | 
|[SetX](./setx/) | Gets or gets the x coordinate of the upper left corner of plot-area bounding box in units of 1/4000 of the chart area. | 
|[GetY](./gety/) | Gets or gets the y coordinate of the upper top corner  of plot-area bounding box in units of 1/4000 of the chart area. | 
|[SetY](./sety/) | Gets or gets the y coordinate of the upper top corner  of plot-area bounding box in units of 1/4000 of the chart area. | 
|[GetHeight](./getheight/) | Gets or sets the height of plot-area bounding box in units of 1/4000 of the chart area. | 
|[SetHeight](./setheight/) | Gets or sets the height of plot-area bounding box in units of 1/4000 of the chart area. | 
|[GetWidth](./getwidth/) | Gets or sets the width of plot-area bounding box in units of 1/4000 of the chart area. | 
|[SetWidth](./setwidth/) | Gets or sets the width of plot-area bounding box in units of 1/4000 of the chart area. | 
|[GetInnerX](./getinnerx/) | Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. | 
|[SetInnerX](./setinnerx/) | Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. | 
|[GetInnerY](./getinnery/) | Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. | 
|[SetInnerY](./setinnery/) | Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. | 
|[GetInnerHeight](./getinnerheight/) | Gets or sets the height of plot area in units of 1/4000 of the chart area. | 
|[SetInnerHeight](./setinnerheight/) | Gets or sets the height of plot area in units of 1/4000 of the chart area. | 
|[GetInnerWidth](./getinnerwidth/) | Gets or sets the width  of plot area in units of 1/4000 of the chart area. | 
|[SetInnerWidth](./setinnerwidth/) | Gets or sets the width  of plot area in units of 1/4000 of the chart area. | 
|[SetPositionAuto](./setpositionauto/) | Set position of the plot area to automatic | 
|[IsAutomaticSize](./isautomaticsize/) | Indicates whether the plot area is automatic sized. | 
|[SetIsAutomaticSize](./setisautomaticsize/) | Indicates whether the plot area is automatic sized. | 
|[IsInnerMode](./isinnermode/) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels.False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. | 
|[SetIsInnerMode](./setisinnermode/) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels.False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. | 
|[GetBackgroundMode](./getbackgroundmode/) | Gets and sets the display mode of the background | 
|[SetBackgroundMode](./setbackgroundmode/) | Gets and sets the display mode of the background | 
|[GetShadow](./getshadow/) | True if the frame has a shadow. | 
|[SetShadow](./setshadow/) | True if the frame has a shadow. | 
|[GetShapeProperties](./getshapeproperties/) | Gets the <see cref="ShapeProperties"/> object. | 
|[IsDefaultPosBeSet](./isdefaultposbeset/) | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. | 
|[GetDefaultX](./getdefaultx/) | Represents x of default position | 
|[GetDefaultY](./getdefaulty/) | Represents y of default position | 
|[GetDefaultWidth](./getdefaultwidth/) | Represents width of default position | 
|[GetDefaultHeight](./getdefaultheight/) | Represents height of default position | 
|[GetBorder](./getborder/) | Gets the <see cref="Line">border</see>. | 
|[GetArea](./getarea/) | Gets the <see cref="Area">area</see>. | 
|[GetTextOptions](./gettextoptions/) | Gets and sets the options of the text. | 
|[GetFont](./getfont/) | Gets a <see cref="Font"/> object of the specified ChartFrame object. | 
|[GetAutoScaleFont](./getautoscalefont/) | True if the text in the object changes font size when the object size changes. The default value is True. | 
|[SetAutoScaleFont](./setautoscalefont/) | True if the text in the object changes font size when the object size changes. The default value is True. | 
