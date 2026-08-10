---
title: "Walls Class"
linktitle: "Walls"
articleTitle: "Walls"
second_title: "Aspose.Cells for Python via Java"
description: "Encapsulates the object that represents the walls of a 3-D chart."
type: docs
weight: 7390
url: /python-java/asposecells.api/walls/
---

## Walls class

Encapsulates the object that represents the walls of a 3-D chart.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [CenterX](#centerx) | int | Gets the x coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's width after calls Chart.Cal |
| [CenterY](#centery) | int | Gets the y coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's height after calls Chart.Ca |
| [Width](#width) | int | Gets the width of left to right in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [Depth](#depth) | int | Gets the depth front to back in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [Height](#height) | int | Gets the height of top to bottom in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [CenterXPx](#centerxpx) | int | Gets the x coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method. |
| [CenterYPx](#centerypx) | int | Gets the y coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method. |
| [WidthPx](#widthpx) | int | Gets the width of left to right in units of pixels after calls Chart.Calculate() method. |
| [DepthPx](#depthpx) | int | Gets the depth front to back in units of pixels after calls Chart.Calculate() method. |
| [HeightPx](#heightpx) | int | Gets the height of top to bottom in units of pixels after calls Chart.Calculate() method. |
| [Border](#border) | Line | Gets or sets the border Line . |
| [BackgroundColor](#backgroundcolor) | Color | Gets or sets the background com.aspose.cells.Color of the Area . |
| [ForegroundColor](#foregroundcolor) | Color | Gets or sets the foreground com.aspose.cells.Color . |
| [Formatting](#formatting) | int | Represents the formatting of the area. The value of the property is FormattingType integer constant. |
| [InvertIfNegative](#invertifnegative) | boolean | If the property is true and the value of chart point is a negative number, the foreground color and background color wil |
| [FillFormat](#fillformat) | FillFormat | Represents a FillFormat object that contains fill formatting properties for the specified chart or shape. |
| [Transparency](#transparency) | float | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |

## Methods

| Name | Description |
| --- | --- |
| [getCubePointCount](#getcubepointcount) | Gets the number of cube points after calls Chart.Calculate() method. |
| [getCubePointXPx](#getcubepointxpx) | Gets x-coordinate of the apex point of walls cube after calls Chart.Calculate() method. The number of apex points of wal |
| [getCubePointYPx](#getcubepointypx) | Gets y-coordinate of the apex point of walls cube after calls Chart.Calculate() method. The number of apex points of wal |

### Walls.CenterX property {#centerx}

Gets the x coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's width after calls Chart.Calculate() method.

**Type:** int

### Walls.CenterY property {#centery}

Gets the y coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's height after calls Chart.Calculate() method.

**Type:** int

### Walls.Width property {#width}

Gets the width of left to right in units of 1/4000 of chart's width after calls Chart.Calculate() method.

**Type:** int

### Walls.Depth property {#depth}

Gets the depth front to back in units of 1/4000 of chart's width after calls Chart.Calculate() method.

**Type:** int

### Walls.Height property {#height}

Gets the height of top to bottom in units of 1/4000 of chart's height after calls Chart.Calculate() method.

**Type:** int

### Walls.CenterXPx property {#centerxpx}

Gets the x coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method.

**Type:** int

### Walls.CenterYPx property {#centerypx}

Gets the y coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method.

**Type:** int

### Walls.WidthPx property {#widthpx}

Gets the width of left to right in units of pixels after calls Chart.Calculate() method.

**Type:** int

### Walls.DepthPx property {#depthpx}

Gets the depth front to back in units of pixels after calls Chart.Calculate() method.

**Type:** int

### Walls.HeightPx property {#heightpx}

Gets the height of top to bottom in units of pixels after calls Chart.Calculate() method.

**Type:** int

### Walls.Border property {#border}

Gets or sets the border Line .

**Type:** Line

### Walls.BackgroundColor property {#backgroundcolor}

Gets or sets the background com.aspose.cells.Color of the Area .

**Type:** Color

### Walls.ForegroundColor property {#foregroundcolor}

Gets or sets the foreground com.aspose.cells.Color .

**Type:** Color

### Walls.Formatting property {#formatting}

Represents the formatting of the area. The value of the property is FormattingType integer constant.

**Type:** int

### Walls.InvertIfNegative property {#invertifnegative}

If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

**Type:** boolean

### Walls.FillFormat property {#fillformat}

Represents a FillFormat object that contains fill formatting properties for the specified chart or shape.

**Type:** FillFormat

### Walls.Transparency property {#transparency}

Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

**Type:** float

### getCubePointCount() {#getcubepointcount}

Gets the number of cube points after calls Chart.Calculate() method.

### getCubePointXPx(index) {#getcubepointxpx}

Gets x-coordinate of the apex point of walls cube after calls Chart.Calculate() method. The number of apex points of walls cube is eight

### getCubePointYPx(index) {#getcubepointypx}

Gets y-coordinate of the apex point of walls cube after calls Chart.Calculate() method. The number of apex points of walls cube is eight.
