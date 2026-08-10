---
title: "ChartFrame Class"
linktitle: "ChartFrame"
articleTitle: "ChartFrame"
second_title: "Aspose.Cells for PHP via Java"
description: "Encapsulates the object that represents the frame object in a chart."
type: docs
weight: 780
url: /php/aspose.cells/chartframe/
---

## ChartFrame class

Encapsulates the object that represents the frame object in a chart.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [IsInnerMode](#isinnermode) | boolean | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the  |
| [Chart](#chart) | Chart | Gets the chart to which this object belongs. |
| [Border](#border) | Line | Gets the Line . |
| [Area](#area) | Area | Gets the Area . |
| [TextFont](#textfont) | Font | Gets a Font object of the specified ChartFrame object. NOTE: This member is now obsolete. Instead, please use ChartFrame |
| [TextOptions](#textoptions) | TextOptions | Gets and sets the options of the text. |
| [Font](#font) | Font | Gets a Font object of the specified ChartFrame object. |
| [AutoScaleFont](#autoscalefont) | boolean | True if the text in the object changes font size when the object size changes. The default value is True. |
| [BackgroundMode](#backgroundmode) | Number | Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant. |
| [Background](#background) | Number | Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant. NOTE: Thi |
| [IsAutomaticSize](#isautomaticsize) | boolean | Indicates whether the chart frame is automatic sized. |
| [X](#x) | Number | Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. How to convert units of 1/4 |
| [Y](#y) | Number | Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. How to convert units of 1/4 |
| [Height](#height) | Number | Gets or sets the height of frame in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Height  |
| [Width](#width) | Number | Gets or sets the width of frame in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Width In |
| [Shadow](#shadow) | boolean | True if the frame has a shadow. |
| [ShapeProperties](#shapeproperties) | ShapePropertyCollection | Gets the ShapeProperties object. |
| [IsDefaultPosBeSet](#isdefaultposbeset) | boolean | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [DefaultX](#defaultx) | Number | Represents x of default position |
| [DefaultY](#defaulty) | Number | Represents y of default position |
| [DefaultWidth](#defaultwidth) | Number | Represents width of default position |
| [DefaultHeight](#defaultheight) | Number | Represents height of default position |
| [DefaultXRatioToChart](#defaultxratiotochart) | Number |  |
| [DefaultYRatioToChart](#defaultyratiotochart) | Number |  |
| [DefaultWidthRatioToChart](#defaultwidthratiotochart) | Number |  |
| [DefaultHeightRatioToChart](#defaultheightratiotochart) | Number |  |
| [XRatioToChart](#xratiotochart) | Number |  |
| [YRatioToChart](#yratiotochart) | Number |  |
| [WidthRatioToChart](#widthratiotochart) | Number |  |
| [HeightRatioToChart](#heightratiotochart) | Number |  |
| [XPixel](#xpixel) | Number |  |
| [YPixel](#ypixel) | Number |  |
| [WidthPixel](#widthpixel) | Number | Represents width |
| [HeightPixel](#heightpixel) | Number | Represents height |

## Methods

| Name | Description |
| --- | --- |
| [setPositionAuto](#setpositionauto) | Set position of the frame to automatic |

### ChartFrame.IsInnerMode property {#isinnermode}

Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. Only for Xlsx file.

**Type:** boolean

### ChartFrame.Chart property {#chart}

Gets the chart to which this object belongs.

**Type:** Chart

### ChartFrame.Border property {#border}

Gets the Line .

**Type:** Line

### ChartFrame.Area property {#area}

Gets the Area .

**Type:** Area

### ChartFrame.TextFont property {#textfont}

Gets a Font object of the specified ChartFrame object. NOTE: This member is now obsolete. Instead, please use ChartFrame.Font property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Type:** Font

### ChartFrame.TextOptions property {#textoptions}

Gets and sets the options of the text.

**Type:** TextOptions

### ChartFrame.Font property {#font}

Gets a Font object of the specified ChartFrame object.

**Type:** Font

### ChartFrame.AutoScaleFont property {#autoscalefont}

True if the text in the object changes font size when the object size changes. The default value is True.

**Type:** boolean

### ChartFrame.BackgroundMode property {#backgroundmode}

Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant.

**Type:** Number

### ChartFrame.Background property {#background}

Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant. NOTE: This member is now obsolete. Instead, please use ChartFrame.BackgroundMode property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Type:** Number

### ChartFrame.IsAutomaticSize property {#isautomaticsize}

Indicates whether the chart frame is automatic sized.

**Type:** boolean

### ChartFrame.X property {#x}

Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? X In Pixels = X * Chart.ChartObject.Width / 4000;

**Type:** Number

### ChartFrame.Y property {#y}

Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Y In Pixels = Y * Chart.ChartObject.Height / 4000;

**Type:** Number

### ChartFrame.Height property {#height}

Gets or sets the height of frame in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Height In Pixels = Y * Chart.ChartObject.Height / 4000;

**Type:** Number

### ChartFrame.Width property {#width}

Gets or sets the width of frame in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Width In Pixels = Width * Chart.ChartObject.Height / 4000;

**Type:** Number

### ChartFrame.Shadow property {#shadow}

True if the frame has a shadow.

**Type:** boolean

### ChartFrame.ShapeProperties property {#shapeproperties}

Gets the ShapeProperties object.

**Type:** ShapePropertyCollection

### ChartFrame.IsDefaultPosBeSet property {#isdefaultposbeset}

Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set.

**Type:** boolean

### ChartFrame.DefaultX property {#defaultx}

Represents x of default position

**Type:** Number

### ChartFrame.DefaultY property {#defaulty}

Represents y of default position

**Type:** Number

### ChartFrame.DefaultWidth property {#defaultwidth}

Represents width of default position

**Type:** Number

### ChartFrame.DefaultHeight property {#defaultheight}

Represents height of default position

**Type:** Number

### ChartFrame.DefaultXRatioToChart property {#defaultxratiotochart}

**Type:** Number

### ChartFrame.DefaultYRatioToChart property {#defaultyratiotochart}

**Type:** Number

### ChartFrame.DefaultWidthRatioToChart property {#defaultwidthratiotochart}

**Type:** Number

### ChartFrame.DefaultHeightRatioToChart property {#defaultheightratiotochart}

**Type:** Number

### ChartFrame.XRatioToChart property {#xratiotochart}

**Type:** Number

### ChartFrame.YRatioToChart property {#yratiotochart}

**Type:** Number

### ChartFrame.WidthRatioToChart property {#widthratiotochart}

**Type:** Number

### ChartFrame.HeightRatioToChart property {#heightratiotochart}

**Type:** Number

### ChartFrame.XPixel property {#xpixel}

**Type:** Number

### ChartFrame.YPixel property {#ypixel}

**Type:** Number

### ChartFrame.WidthPixel property {#widthpixel}

Represents width

**Type:** Number

### ChartFrame.HeightPixel property {#heightpixel}

Represents height

**Type:** Number

### setPositionAuto() {#setpositionauto}

Set position of the frame to automatic
