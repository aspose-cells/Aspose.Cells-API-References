---
title: ChartFrame Class 
linktitle: ChartFrame
second_title: Aspose.Cells for Go via C++ API Reference
description: 'ChartFrame class. Encapsulates the object that represents chartframe in Go.'
type: docs
weight: 200
url: /go-cpp/chartframe/
---

## ChartFrame class

Encapsulates the object that represents the frame object in a chart.

```go

type ChartFrame struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
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
|[IsAutomaticSize](./isautomaticsize/) | Indicates whether the chart frame is automatic sized. | 
|[SetIsAutomaticSize](./setisautomaticsize/) | Indicates whether the chart frame is automatic sized. | 
|[GetX](./getx/) | Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. | 
|[SetX](./setx/) | Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. | 
|[GetY](./gety/) | Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. | 
|[SetY](./sety/) | Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. | 
|[GetHeight](./getheight/) | Gets or sets the height of frame in units of 1/4000 of the chart area. | 
|[SetHeight](./setheight/) | Gets or sets the height of frame in units of 1/4000 of the chart area. | 
|[GetWidth](./getwidth/) | Gets or sets the width of frame in units of 1/4000 of the chart area. | 
|[SetWidth](./setwidth/) | Gets or sets the width of frame in units of 1/4000 of the chart area. | 
|[SetPositionAuto](./setpositionauto/) | Set position of the frame to automatic | 
