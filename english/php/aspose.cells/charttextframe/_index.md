---
title: "ChartTextFrame Class"
linktitle: "ChartTextFrame"
articleTitle: "ChartTextFrame"
second_title: "Aspose.Cells for PHP via Java"
description: "Encapsulates the object that represents the frame object which contains text."
type: docs
weight: 870
url: /php/aspose.cells/charttextframe/
---

## ChartTextFrame class

Encapsulates the object that represents the frame object which contains text.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [IsAutoText](#isautotext) | boolean | Indicates the text is auto generated. |
| [IsDeleted](#isdeleted) | boolean | Indicates whether this data labels is deleted. |
| [TextHorizontalAlignment](#texthorizontalalignment) | Number | Gets and sets the text horizontal alignment. The value of the property is TextAlignmentType integer constant. |
| [TextVerticalAlignment](#textverticalalignment) | Number | Gets or sets the text vertical alignment of text. The value of the property is TextAlignmentType integer constant. |
| [RotationAngle](#rotationangle) | Number | Represents text rotation angle. 0: Not rotated. 255: Top to Bottom. -90: Downward. 90: Upward. |
| [IsAutomaticRotation](#isautomaticrotation) | boolean | Indicates whether the text of the chart is automatically rotated. |
| [Text](#text) | String | Gets or sets the text of a frame's title. |
| [LinkedSource](#linkedsource) | String | Gets and sets a reference to the worksheet. |
| [TextDirection](#textdirection) | Number | Represents text reading order. The value of the property is TextDirectionType integer constant. NOTE: This member is now |
| [ReadingOrder](#readingorder) | Number | Represents text reading order. The value of the property is TextDirectionType integer constant. |
| [DirectionType](#directiontype) | Number | Gets and sets the direction of text. The value of the property is ChartTextDirectionType integer constant. |
| [IsTextWrapped](#istextwrapped) | boolean | Gets or sets a value indicating whether the text is wrapped. |
| [IsResizeShapeToFitText](#isresizeshapetofittext) | boolean | Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text |
| [IsInnerMode](#isinnermode) | boolean | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the  |
| [Chart](#chart) | Chart | Gets the chart to which this object belongs. |
| [Border](#border) | Line | Gets the Line . |
| [Area](#area) | Area | Gets the area . |
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
| [characters](#characters) | Returns a Characters object that represents a range of characters within the text. |
| [setPositionAuto](#setpositionauto) | Set position of the frame to automatic |

### ChartTextFrame.IsAutoText property {#isautotext}

Indicates the text is auto generated.

**Type:** boolean

### ChartTextFrame.IsDeleted property {#isdeleted}

Indicates whether this data labels is deleted.

**Type:** boolean

### ChartTextFrame.TextHorizontalAlignment property {#texthorizontalalignment}

Gets and sets the text horizontal alignment. The value of the property is TextAlignmentType integer constant.

**Type:** Number

### ChartTextFrame.TextVerticalAlignment property {#textverticalalignment}

Gets or sets the text vertical alignment of text. The value of the property is TextAlignmentType integer constant.

**Type:** Number

### ChartTextFrame.RotationAngle property {#rotationangle}

Represents text rotation angle. 0: Not rotated. 255: Top to Bottom. -90: Downward. 90: Upward.

**Type:** Number

### ChartTextFrame.IsAutomaticRotation property {#isautomaticrotation}

Indicates whether the text of the chart is automatically rotated.

**Type:** boolean

### ChartTextFrame.Text property {#text}

Gets or sets the text of a frame's title.

**Type:** String

### ChartTextFrame.LinkedSource property {#linkedsource}

Gets and sets a reference to the worksheet.

**Type:** String

### ChartTextFrame.TextDirection property {#textdirection}

Represents text reading order. The value of the property is TextDirectionType integer constant. NOTE: This member is now obsolete. Instead, please use ChartTextFrame.ReadingOrder property. This property will be removed 12 months later since March 2020. Aspose apologizes for any inconvenience you may have experienced.

**Type:** Number

### ChartTextFrame.ReadingOrder property {#readingorder}

Represents text reading order. The value of the property is TextDirectionType integer constant.

**Type:** Number

### ChartTextFrame.DirectionType property {#directiontype}

Gets and sets the direction of text. The value of the property is ChartTextDirectionType integer constant.

**Type:** Number

### ChartTextFrame.IsTextWrapped property {#istextwrapped}

Gets or sets a value indicating whether the text is wrapped.

**Type:** boolean

### ChartTextFrame.IsResizeShapeToFitText property {#isresizeshapetofittext}

Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside.

**Type:** boolean

### ChartTextFrame.IsInnerMode property {#isinnermode}

Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. Only for Xlsx file.

**Type:** boolean

### ChartTextFrame.Chart property {#chart}

Gets the chart to which this object belongs.

**Type:** Chart

### ChartTextFrame.Border property {#border}

Gets the Line .

**Type:** Line

### ChartTextFrame.Area property {#area}

Gets the area .

**Type:** Area

### ChartTextFrame.TextFont property {#textfont}

Gets a Font object of the specified ChartFrame object. NOTE: This member is now obsolete. Instead, please use ChartFrame.Font property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Type:** Font

### ChartTextFrame.TextOptions property {#textoptions}

Gets and sets the options of the text.

**Type:** TextOptions

### ChartTextFrame.Font property {#font}

Gets a Font object of the specified ChartFrame object.

**Type:** Font

### ChartTextFrame.AutoScaleFont property {#autoscalefont}

True if the text in the object changes font size when the object size changes. The default value is True.

**Type:** boolean

### ChartTextFrame.BackgroundMode property {#backgroundmode}

Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant.

**Type:** Number

### ChartTextFrame.Background property {#background}

Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant. NOTE: This member is now obsolete. Instead, please use ChartFrame.BackgroundMode property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Type:** Number

### ChartTextFrame.IsAutomaticSize property {#isautomaticsize}

Indicates whether the chart frame is automatic sized.

**Type:** boolean

### ChartTextFrame.X property {#x}

Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? X In Pixels = X * Chart.ChartObject.Width / 4000;

**Type:** Number

### ChartTextFrame.Y property {#y}

Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Y In Pixels = Y * Chart.ChartObject.Height / 4000;

**Type:** Number

### ChartTextFrame.Height property {#height}

Gets or sets the height of frame in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Height In Pixels = Y * Chart.ChartObject.Height / 4000;

**Type:** Number

### ChartTextFrame.Width property {#width}

Gets or sets the width of frame in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Width In Pixels = Width * Chart.ChartObject.Height / 4000;

**Type:** Number

### ChartTextFrame.Shadow property {#shadow}

True if the frame has a shadow.

**Type:** boolean

### ChartTextFrame.ShapeProperties property {#shapeproperties}

Gets the ShapeProperties object.

**Type:** ShapePropertyCollection

### ChartTextFrame.IsDefaultPosBeSet property {#isdefaultposbeset}

Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set.

**Type:** boolean

### ChartTextFrame.DefaultX property {#defaultx}

Represents x of default position

**Type:** Number

### ChartTextFrame.DefaultY property {#defaulty}

Represents y of default position

**Type:** Number

### ChartTextFrame.DefaultWidth property {#defaultwidth}

Represents width of default position

**Type:** Number

### ChartTextFrame.DefaultHeight property {#defaultheight}

Represents height of default position

**Type:** Number

### ChartTextFrame.DefaultXRatioToChart property {#defaultxratiotochart}

**Type:** Number

### ChartTextFrame.DefaultYRatioToChart property {#defaultyratiotochart}

**Type:** Number

### ChartTextFrame.DefaultWidthRatioToChart property {#defaultwidthratiotochart}

**Type:** Number

### ChartTextFrame.DefaultHeightRatioToChart property {#defaultheightratiotochart}

**Type:** Number

### ChartTextFrame.XRatioToChart property {#xratiotochart}

**Type:** Number

### ChartTextFrame.YRatioToChart property {#yratiotochart}

**Type:** Number

### ChartTextFrame.WidthRatioToChart property {#widthratiotochart}

**Type:** Number

### ChartTextFrame.HeightRatioToChart property {#heightratiotochart}

**Type:** Number

### ChartTextFrame.XPixel property {#xpixel}

**Type:** Number

### ChartTextFrame.YPixel property {#ypixel}

**Type:** Number

### ChartTextFrame.WidthPixel property {#widthpixel}

Represents width

**Type:** Number

### ChartTextFrame.HeightPixel property {#heightpixel}

Represents height

**Type:** Number

### characters(startIndex, length) {#characters}

Returns a Characters object that represents a range of characters within the text.

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Number | The index of the start of the character. |
| length | Number | The number of characters. |

**Returns:** Characters object.

### setPositionAuto() {#setpositionauto}

Set position of the frame to automatic
