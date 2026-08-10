---
title: "DisplayUnitLabel Class"
linktitle: "DisplayUnitLabel"
articleTitle: "DisplayUnitLabel"
second_title: "Aspose.Cells for Python via Java"
description: "Represents the display unit label."
type: docs
weight: 1810
url: /python-java/asposecells.api/displayunitlabel/
---

## DisplayUnitLabel class

Represents the display unit label.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Text](#text) | String | Gets or sets the text of display unit label. |
| [Font](#font) | Font | Gets a Font object of the specified ChartFrame object. |
| [AutoScaleFont](#autoscalefont) | boolean | True if the text in the object changes font size when the object size changes. The default value is True. |
| [IsAutoText](#isautotext) | boolean | Indicates the text is auto generated. |
| [IsDeleted](#isdeleted) | boolean | Indicates whether this data labels is deleted. |
| [TextHorizontalAlignment](#texthorizontalalignment) | int | Gets and sets the text horizontal alignment. The value of the property is TextAlignmentType integer constant. |
| [TextVerticalAlignment](#textverticalalignment) | int | Gets or sets the text vertical alignment of text. The value of the property is TextAlignmentType integer constant. |
| [RotationAngle](#rotationangle) | int | Represents text rotation angle. 0: Not rotated. 255: Top to Bottom. -90: Downward. 90: Upward. |
| [IsAutomaticRotation](#isautomaticrotation) | boolean | Indicates whether the text of the chart is automatically rotated. |
| [LinkedSource](#linkedsource) | String | Gets and sets a reference to the worksheet. |
| [TextDirection](#textdirection) | int | Represents text reading order. The value of the property is TextDirectionType integer constant. NOTE: This member is now |
| [ReadingOrder](#readingorder) | int | Represents text reading order. The value of the property is TextDirectionType integer constant. |
| [DirectionType](#directiontype) | int | Gets and sets the direction of text. The value of the property is ChartTextDirectionType integer constant. |
| [IsTextWrapped](#istextwrapped) | boolean | Gets or sets a value indicating whether the text is wrapped. |
| [IsResizeShapeToFitText](#isresizeshapetofittext) | boolean | Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text |
| [IsInnerMode](#isinnermode) | boolean | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the  |
| [Chart](#chart) | Chart | Gets the chart to which this object belongs. |
| [Border](#border) | Line | Gets the Line . |
| [Area](#area) | Area | Gets the area . |
| [TextFont](#textfont) | Font | Gets a Font object of the specified ChartFrame object. NOTE: This member is now obsolete. Instead, please use ChartFrame |
| [TextOptions](#textoptions) | TextOptions | Gets and sets the options of the text. |
| [BackgroundMode](#backgroundmode) | int | Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant. |
| [Background](#background) | int | Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant. NOTE: Thi |
| [IsAutomaticSize](#isautomaticsize) | boolean | Indicates whether the chart frame is automatic sized. |
| [X](#x) | int | Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. How to convert units of 1/4 |
| [Y](#y) | int | Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. How to convert units of 1/4 |
| [Height](#height) | int | Gets or sets the height of frame in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Height  |
| [Width](#width) | int | Gets or sets the width of frame in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Width In |
| [Shadow](#shadow) | boolean | True if the frame has a shadow. |
| [ShapeProperties](#shapeproperties) | ShapePropertyCollection | Gets the ShapeProperties object. |
| [IsDefaultPosBeSet](#isdefaultposbeset) | boolean | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [DefaultX](#defaultx) | int | Represents x of default position |
| [DefaultY](#defaulty) | int | Represents y of default position |
| [DefaultWidth](#defaultwidth) | int | Represents width of default position |
| [DefaultHeight](#defaultheight) | int | Represents height of default position |
| [DefaultXRatioToChart](#defaultxratiotochart) | float |  |
| [DefaultYRatioToChart](#defaultyratiotochart) | float |  |
| [DefaultWidthRatioToChart](#defaultwidthratiotochart) | float |  |
| [DefaultHeightRatioToChart](#defaultheightratiotochart) | float |  |
| [XRatioToChart](#xratiotochart) | float |  |
| [YRatioToChart](#yratiotochart) | float |  |
| [WidthRatioToChart](#widthratiotochart) | float |  |
| [HeightRatioToChart](#heightratiotochart) | float |  |
| [XPixel](#xpixel) | int |  |
| [YPixel](#ypixel) | int |  |
| [WidthPixel](#widthpixel) | int | Represents width |
| [HeightPixel](#heightpixel) | int | Represents height |

## Methods

| Name | Description |
| --- | --- |
| [characters](#characters) | Returns a Characters object that represents a range of characters within the text. |
| [setPositionAuto](#setpositionauto) | Set position of the frame to automatic |

### DisplayUnitLabel.Text property {#text}

Gets or sets the text of display unit label.

**Type:** String

### DisplayUnitLabel.Font property {#font}

Gets a Font object of the specified ChartFrame object.

**Type:** Font

### DisplayUnitLabel.AutoScaleFont property {#autoscalefont}

True if the text in the object changes font size when the object size changes. The default value is True.

**Type:** boolean

### DisplayUnitLabel.IsAutoText property {#isautotext}

Indicates the text is auto generated.

**Type:** boolean

### DisplayUnitLabel.IsDeleted property {#isdeleted}

Indicates whether this data labels is deleted.

**Type:** boolean

### DisplayUnitLabel.TextHorizontalAlignment property {#texthorizontalalignment}

Gets and sets the text horizontal alignment. The value of the property is TextAlignmentType integer constant.

**Type:** int

### DisplayUnitLabel.TextVerticalAlignment property {#textverticalalignment}

Gets or sets the text vertical alignment of text. The value of the property is TextAlignmentType integer constant.

**Type:** int

### DisplayUnitLabel.RotationAngle property {#rotationangle}

Represents text rotation angle. 0: Not rotated. 255: Top to Bottom. -90: Downward. 90: Upward.

**Type:** int

### DisplayUnitLabel.IsAutomaticRotation property {#isautomaticrotation}

Indicates whether the text of the chart is automatically rotated.

**Type:** boolean

### DisplayUnitLabel.LinkedSource property {#linkedsource}

Gets and sets a reference to the worksheet.

**Type:** String

### DisplayUnitLabel.TextDirection property {#textdirection}

Represents text reading order. The value of the property is TextDirectionType integer constant. NOTE: This member is now obsolete. Instead, please use ChartTextFrame.ReadingOrder property. This property will be removed 12 months later since March 2020. Aspose apologizes for any inconvenience you may have experienced.

**Type:** int

### DisplayUnitLabel.ReadingOrder property {#readingorder}

Represents text reading order. The value of the property is TextDirectionType integer constant.

**Type:** int

### DisplayUnitLabel.DirectionType property {#directiontype}

Gets and sets the direction of text. The value of the property is ChartTextDirectionType integer constant.

**Type:** int

### DisplayUnitLabel.IsTextWrapped property {#istextwrapped}

Gets or sets a value indicating whether the text is wrapped.

**Type:** boolean

### DisplayUnitLabel.IsResizeShapeToFitText property {#isresizeshapetofittext}

Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside.

**Type:** boolean

### DisplayUnitLabel.IsInnerMode property {#isinnermode}

Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. Only for Xlsx file.

**Type:** boolean

### DisplayUnitLabel.Chart property {#chart}

Gets the chart to which this object belongs.

**Type:** Chart

### DisplayUnitLabel.Border property {#border}

Gets the Line .

**Type:** Line

### DisplayUnitLabel.Area property {#area}

Gets the area .

**Type:** Area

### DisplayUnitLabel.TextFont property {#textfont}

Gets a Font object of the specified ChartFrame object. NOTE: This member is now obsolete. Instead, please use ChartFrame.Font property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Type:** Font

### DisplayUnitLabel.TextOptions property {#textoptions}

Gets and sets the options of the text.

**Type:** TextOptions

### DisplayUnitLabel.BackgroundMode property {#backgroundmode}

Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant.

**Type:** int

### DisplayUnitLabel.Background property {#background}

Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant. NOTE: This member is now obsolete. Instead, please use ChartFrame.BackgroundMode property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Type:** int

### DisplayUnitLabel.IsAutomaticSize property {#isautomaticsize}

Indicates whether the chart frame is automatic sized.

**Type:** boolean

### DisplayUnitLabel.X property {#x}

Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? X In Pixels = X * Chart.ChartObject.Width / 4000;

**Type:** int

### DisplayUnitLabel.Y property {#y}

Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Y In Pixels = Y * Chart.ChartObject.Height / 4000;

**Type:** int

### DisplayUnitLabel.Height property {#height}

Gets or sets the height of frame in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Height In Pixels = Y * Chart.ChartObject.Height / 4000;

**Type:** int

### DisplayUnitLabel.Width property {#width}

Gets or sets the width of frame in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Width In Pixels = Width * Chart.ChartObject.Height / 4000;

**Type:** int

### DisplayUnitLabel.Shadow property {#shadow}

True if the frame has a shadow.

**Type:** boolean

### DisplayUnitLabel.ShapeProperties property {#shapeproperties}

Gets the ShapeProperties object.

**Type:** ShapePropertyCollection

### DisplayUnitLabel.IsDefaultPosBeSet property {#isdefaultposbeset}

Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set.

**Type:** boolean

### DisplayUnitLabel.DefaultX property {#defaultx}

Represents x of default position

**Type:** int

### DisplayUnitLabel.DefaultY property {#defaulty}

Represents y of default position

**Type:** int

### DisplayUnitLabel.DefaultWidth property {#defaultwidth}

Represents width of default position

**Type:** int

### DisplayUnitLabel.DefaultHeight property {#defaultheight}

Represents height of default position

**Type:** int

### DisplayUnitLabel.DefaultXRatioToChart property {#defaultxratiotochart}

**Type:** float

### DisplayUnitLabel.DefaultYRatioToChart property {#defaultyratiotochart}

**Type:** float

### DisplayUnitLabel.DefaultWidthRatioToChart property {#defaultwidthratiotochart}

**Type:** float

### DisplayUnitLabel.DefaultHeightRatioToChart property {#defaultheightratiotochart}

**Type:** float

### DisplayUnitLabel.XRatioToChart property {#xratiotochart}

**Type:** float

### DisplayUnitLabel.YRatioToChart property {#yratiotochart}

**Type:** float

### DisplayUnitLabel.WidthRatioToChart property {#widthratiotochart}

**Type:** float

### DisplayUnitLabel.HeightRatioToChart property {#heightratiotochart}

**Type:** float

### DisplayUnitLabel.XPixel property {#xpixel}

**Type:** int

### DisplayUnitLabel.YPixel property {#ypixel}

**Type:** int

### DisplayUnitLabel.WidthPixel property {#widthpixel}

Represents width

**Type:** int

### DisplayUnitLabel.HeightPixel property {#heightpixel}

Represents height

**Type:** int

### characters(startIndex, length) {#characters}

Returns a Characters object that represents a range of characters within the text.

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int | The index of the start of the character. |
| length | int | The number of characters. |

**Returns:** Characters object.

### setPositionAuto() {#setpositionauto}

Set position of the frame to automatic
