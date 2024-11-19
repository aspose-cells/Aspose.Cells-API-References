---
title: Walls Class 
linktitle: Walls
second_title: Aspose.Cells for Go API Reference
description: 'Walls class. Encapsulates the object that represents walls in Go.'
type: docs
weight: 200
url: /go/aspose.cells.charts/walls/
---

## Walls class

Encapsulates the object that represents the walls of a 3-D chart.

```go

type Walls struct 

walls, _ := asposecells.NewWalls()

```
## Constructors

| Method | Description |
| --- | --- |
|[NewWalls_Walls](./newwalls_walls/) | Constructs from an implementation object. | 
|[NewWalls_Floor](./newwalls_floor/) | Constructs from a parent object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetCenterX](./getcenterx/) | Gets the x coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's width after calls Chart.Calculate() method. | 
|[GetCenterY](./getcentery/) | Gets the y coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's height after calls Chart.Calculate() method. | 
|[GetWidth](./getwidth/) | Gets the width of left to right in units of 1/4000 of chart's width after calls Chart.Calculate() method. | 
|[GetDepth](./getdepth/) | Gets the depth front to back in units of 1/4000 of chart's width after calls Chart.Calculate() method. | 
|[GetHeight](./getheight/) | Gets the height of top to bottom in units of 1/4000 of chart's height after calls Chart.Calculate() method. | 
|[GetCenterXPx](./getcenterxpx/) | Gets the x coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method. | 
|[GetCenterYPx](./getcenterypx/) | Gets the y coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method. | 
|[GetWidthPx](./getwidthpx/) | Gets the width of left to right in units of pixels after calls Chart.Calculate() method. | 
|[GetDepthPx](./getdepthpx/) | Gets the depth front to back in units of pixels after calls Chart.Calculate() method. | 
|[GetHeightPx](./getheightpx/) | Gets the height of top to bottom in units of pixels after calls Chart.Calculate() method. | 
|[GetCubePointCount](./getcubepointcount/) | Gets the number of cube points after calls Chart.Calculate() method. | 
|[GetCubePointXPx](./getcubepointxpx/) | Gets x-coordinate of the apex point of walls cube after calls Chart.Calculate() method.The number of apex points of walls cube is eight | 
|[GetCubePointYPx](./getcubepointypx/) | Gets y-coordinate of the apex point of walls cube after calls Chart.Calculate() method.The number of apex points of walls cube is eight. | 
|[GetBorder](./getborder/) | Gets or sets the border <see cref="Line"/>. | 
|[SetBorder](./setborder/) | Gets or sets the border <see cref="Line"/>. | 
