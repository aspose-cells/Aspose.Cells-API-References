---
title: ChartArea Class 
linktitle: ChartArea
second_title: Aspose.Cells for Go API Reference
description: 'ChartArea class. Encapsulates the object that represents chartarea in Go.'
type: docs
weight: 200
url: /go/aspose.cells.charts/chartarea/
---

## ChartArea class

Encapsulates the object that represents the chart area in the worksheet.

```go

type ChartArea struct 

chartarea, _ := asposecells.NewChartArea()

```
## Constructors

| Method | Description |
| --- | --- |
|[NewChartArea_ChartArea](./newchartarea_chartarea/) | Constructs from an implementation object. | 
|[NewChartArea_ChartFrame](./newchartarea_chartframe/) | Constructs from a parent object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetX](./getx/) | Gets or gets the horizontal offset from its upper left corner column. | 
|[SetX](./setx/) | Gets or gets the horizontal offset from its upper left corner column. | 
|[GetY](./gety/) | Gets or gets the vertical offset from its upper left corner row. | 
|[SetY](./sety/) | Gets or gets the vertical offset from its upper left corner row. | 
|[GetHeight](./getheight/) | Gets or sets the vertical offset from its lower right corner row. | 
|[SetHeight](./setheight/) | Gets or sets the vertical offset from its lower right corner row. | 
|[GetWidth](./getwidth/) | Gets or sets the horizontal offset from its lower right corner column. | 
|[SetWidth](./setwidth/) | Gets or sets the horizontal offset from its lower right corner column. | 
|[GetFont](./getfont/) | Gets a <see cref="Font"/> object of the specified chartarea object. | 
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
|[GetAutoScaleFont](./getautoscalefont/) | True if the text in the object changes font size when the object size changes. The default value is True. | 
|[SetAutoScaleFont](./setautoscalefont/) | True if the text in the object changes font size when the object size changes. The default value is True. | 
|[IsAutomaticSize](./isautomaticsize/) | Indicates whether the chart frame is automatic sized. | 
|[SetIsAutomaticSize](./setisautomaticsize/) | Indicates whether the chart frame is automatic sized. | 
|[SetPositionAuto](./setpositionauto/) | Set position of the frame to automatic | 
