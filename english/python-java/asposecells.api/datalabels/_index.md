---
title: "DataLabels Class"
linktitle: "DataLabels"
articleTitle: "DataLabels"
second_title: "Aspose.Cells for Python via Java"
description: "Encapsulates a collection of all the DataLabel objects for the specified Series."
type: docs
weight: 1570
url: /python-java/asposecells.api/datalabels/
---

## DataLabels class

Encapsulates a collection of all the DataLabel objects for the specified Series.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Border](#border) | Line | Gets the Line . |
| [Area](#area) | Area | Gets the Area . |
| [IsAutoText](#isautotext) | boolean | Indicates the text is auto generated. |
| [DirectionType](#directiontype) | int | Gets and sets the direction of text. The value of the property is ChartTextDirectionType integer constant. |
| [Text](#text) | String | Gets or sets the text of data label. |
| [IsTextWrapped](#istextwrapped) | boolean | Gets or sets a value indicating whether the text is wrapped. |
| [BackgroundMode](#backgroundmode) | int | Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant. |
| [ShowValue](#showvalue) | boolean | Represents a specified chart's data label values display behavior. True displays the values. False to hide. |
| [ShowCellRange](#showcellrange) | boolean | Indicates whether showing cell range as the data labels. |
| [ShowPercentage](#showpercentage) | boolean | Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False t |
| [ShowBubbleSize](#showbubblesize) | boolean | Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False t |
| [ShowCategoryName](#showcategoryname) | boolean | Represents a specified chart's data label category name display behavior.True to display the category name for the data  |
| [ShowSeriesName](#showseriesname) | boolean | Indicates whether the series name displays for the data labels on a chart. True to show the series name. False to hide. |
| [ShowLegendKey](#showlegendkey) | boolean | Represents a specified chart's data label legend key display behavior. True if the data label legend key is visible. |
| [NumberFormat](#numberformat) | String | Represents the format string for the DataLabels object. |
| [Number](#number) | int | Gets and sets the built-in number format. |
| [NumberFormatLinked](#numberformatlinked) | boolean | True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the |
| [Font](#font) | Font | Gets the font of the DataLabels; |
| [SeparatorType](#separatortype) | int | Gets or sets the separator type used for the data labels on a chart. The value of the property is DataLabelsSeparatorTyp |
| [SeparatorValue](#separatorvalue) | String | Gets or sets the separator value used for the data labels on a chart. |
| [Position](#position) | int | Represents the position of the data label. The value of the property is LabelPositionType integer constant. |
| [IsNeverOverlap](#isneveroverlap) | boolean | Indicates whether the datalabels display never overlap. (For Pie chart) |
| [ShapeType](#shapetype) | int | Gets or sets shape type of data label. The value of the property is DataLabelShapeType integer constant. |
| [IsDeleted](#isdeleted) | boolean | Indicates whether this data labels is deleted. |
| [TextHorizontalAlignment](#texthorizontalalignment) | int | Gets and sets the text horizontal alignment. The value of the property is TextAlignmentType integer constant. |
| [TextVerticalAlignment](#textverticalalignment) | int | Gets or sets the text vertical alignment of text. The value of the property is TextAlignmentType integer constant. |
| [RotationAngle](#rotationangle) | int | Represents text rotation angle. 0: Not rotated. 255: Top to Bottom. -90: Downward. 90: Upward. |
| [IsAutomaticRotation](#isautomaticrotation) | boolean | Indicates whether the text of the chart is automatically rotated. |
| [LinkedSource](#linkedsource) | String | Gets and sets a reference to the worksheet. |
| [TextDirection](#textdirection) | int | Represents text reading order. The value of the property is TextDirectionType integer constant. NOTE: This member is now |
| [ReadingOrder](#readingorder) | int | Represents text reading order. The value of the property is TextDirectionType integer constant. |
| [IsResizeShapeToFitText](#isresizeshapetofittext) | boolean | Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text |
| [IsInnerMode](#isinnermode) | boolean | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the  |
| [Chart](#chart) | Chart | Gets the chart to which this object belongs. |
| [TextFont](#textfont) | Font | Gets a Font object of the specified ChartFrame object. NOTE: This member is now obsolete. Instead, please use ChartFrame |
| [TextOptions](#textoptions) | TextOptions | Gets and sets the options of the text. |
| [AutoScaleFont](#autoscalefont) | boolean | True if the text in the object changes font size when the object size changes. The default value is True. |
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
| [applyFont](#applyfont) | Apply the font of the datalabels to all child nodes. |
| [characters](#characters) | Returns a Characters object that represents a range of characters within the text. |
| [setPositionAuto](#setpositionauto) | Set position of the frame to automatic |

### DataLabels.Border property {#border}

Gets the Line .

**Type:** Line

### DataLabels.Area property {#area}

Gets the Area .

**Type:** Area

### DataLabels.IsAutoText property {#isautotext}

Indicates the text is auto generated.

**Type:** boolean

### DataLabels.DirectionType property {#directiontype}

Gets and sets the direction of text. The value of the property is ChartTextDirectionType integer constant.

**Type:** int

### DataLabels.Text property {#text}

Gets or sets the text of data label.

**Type:** String

### DataLabels.IsTextWrapped property {#istextwrapped}

Gets or sets a value indicating whether the text is wrapped.

**Type:** boolean

### DataLabels.BackgroundMode property {#backgroundmode}

Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant.

**Type:** int

### DataLabels.ShowValue property {#showvalue}

Represents a specified chart's data label values display behavior. True displays the values. False to hide.

**Type:** boolean

### DataLabels.ShowCellRange property {#showcellrange}

Indicates whether showing cell range as the data labels.

**Type:** boolean

### DataLabels.ShowPercentage property {#showpercentage}

Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide.

**Type:** boolean

### DataLabels.ShowBubbleSize property {#showbubblesize}

Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide.

**Type:** boolean

### DataLabels.ShowCategoryName property {#showcategoryname}

Represents a specified chart's data label category name display behavior.True to display the category name for the data labels on a chart. False to hide.

**Type:** boolean

### DataLabels.ShowSeriesName property {#showseriesname}

Indicates whether the series name displays for the data labels on a chart. True to show the series name. False to hide.

**Type:** boolean

### DataLabels.ShowLegendKey property {#showlegendkey}

Represents a specified chart's data label legend key display behavior. True if the data label legend key is visible.

**Type:** boolean

### DataLabels.NumberFormat property {#numberformat}

Represents the format string for the DataLabels object.

**Type:** String

### DataLabels.Number property {#number}

Gets and sets the built-in number format.

**Type:** int

### DataLabels.NumberFormatLinked property {#numberformatlinked}

True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells).

**Type:** boolean

### DataLabels.Font property {#font}

Gets the font of the DataLabels;

**Type:** Font

### DataLabels.SeparatorType property {#separatortype}

Gets or sets the separator type used for the data labels on a chart. The value of the property is DataLabelsSeparatorType integer constant. To set custom separator, please set the property SeparatorType as DataLabelsSeparatorType.CUSTOM and then specify the expected value for SeparatorValue .

**Type:** int

### DataLabels.SeparatorValue property {#separatorvalue}

Gets or sets the separator value used for the data labels on a chart.

**Type:** String

### DataLabels.Position property {#position}

Represents the position of the data label. The value of the property is LabelPositionType integer constant.

**Type:** int

### DataLabels.IsNeverOverlap property {#isneveroverlap}

Indicates whether the datalabels display never overlap. (For Pie chart)

**Type:** boolean

### DataLabels.ShapeType property {#shapetype}

Gets or sets shape type of data label. The value of the property is DataLabelShapeType integer constant.

**Type:** int

### DataLabels.IsDeleted property {#isdeleted}

Indicates whether this data labels is deleted.

**Type:** boolean

### DataLabels.TextHorizontalAlignment property {#texthorizontalalignment}

Gets and sets the text horizontal alignment. The value of the property is TextAlignmentType integer constant.

**Type:** int

### DataLabels.TextVerticalAlignment property {#textverticalalignment}

Gets or sets the text vertical alignment of text. The value of the property is TextAlignmentType integer constant.

**Type:** int

### DataLabels.RotationAngle property {#rotationangle}

Represents text rotation angle. 0: Not rotated. 255: Top to Bottom. -90: Downward. 90: Upward.

**Type:** int

### DataLabels.IsAutomaticRotation property {#isautomaticrotation}

Indicates whether the text of the chart is automatically rotated.

**Type:** boolean

### DataLabels.LinkedSource property {#linkedsource}

Gets and sets a reference to the worksheet.

**Type:** String

### DataLabels.TextDirection property {#textdirection}

Represents text reading order. The value of the property is TextDirectionType integer constant. NOTE: This member is now obsolete. Instead, please use ChartTextFrame.ReadingOrder property. This property will be removed 12 months later since March 2020. Aspose apologizes for any inconvenience you may have experienced.

**Type:** int

### DataLabels.ReadingOrder property {#readingorder}

Represents text reading order. The value of the property is TextDirectionType integer constant.

**Type:** int

### DataLabels.IsResizeShapeToFitText property {#isresizeshapetofittext}

Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside.

**Type:** boolean

### DataLabels.IsInnerMode property {#isinnermode}

Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. Only for Xlsx file.

**Type:** boolean

### DataLabels.Chart property {#chart}

Gets the chart to which this object belongs.

**Type:** Chart

### DataLabels.TextFont property {#textfont}

Gets a Font object of the specified ChartFrame object. NOTE: This member is now obsolete. Instead, please use ChartFrame.Font property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Type:** Font

### DataLabels.TextOptions property {#textoptions}

Gets and sets the options of the text.

**Type:** TextOptions

### DataLabels.AutoScaleFont property {#autoscalefont}

True if the text in the object changes font size when the object size changes. The default value is True.

**Type:** boolean

### DataLabels.Background property {#background}

Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant. NOTE: This member is now obsolete. Instead, please use ChartFrame.BackgroundMode property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Type:** int

### DataLabels.IsAutomaticSize property {#isautomaticsize}

Indicates whether the chart frame is automatic sized.

**Type:** boolean

### DataLabels.X property {#x}

Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? X In Pixels = X * Chart.ChartObject.Width / 4000;

**Type:** int

### DataLabels.Y property {#y}

Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Y In Pixels = Y * Chart.ChartObject.Height / 4000;

**Type:** int

### DataLabels.Height property {#height}

Gets or sets the height of frame in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Height In Pixels = Y * Chart.ChartObject.Height / 4000;

**Type:** int

### DataLabels.Width property {#width}

Gets or sets the width of frame in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Width In Pixels = Width * Chart.ChartObject.Height / 4000;

**Type:** int

### DataLabels.Shadow property {#shadow}

True if the frame has a shadow.

**Type:** boolean

### DataLabels.ShapeProperties property {#shapeproperties}

Gets the ShapeProperties object.

**Type:** ShapePropertyCollection

### DataLabels.IsDefaultPosBeSet property {#isdefaultposbeset}

Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set.

**Type:** boolean

### DataLabels.DefaultX property {#defaultx}

Represents x of default position

**Type:** int

### DataLabels.DefaultY property {#defaulty}

Represents y of default position

**Type:** int

### DataLabels.DefaultWidth property {#defaultwidth}

Represents width of default position

**Type:** int

### DataLabels.DefaultHeight property {#defaultheight}

Represents height of default position

**Type:** int

### DataLabels.DefaultXRatioToChart property {#defaultxratiotochart}

**Type:** float

### DataLabels.DefaultYRatioToChart property {#defaultyratiotochart}

**Type:** float

### DataLabels.DefaultWidthRatioToChart property {#defaultwidthratiotochart}

**Type:** float

### DataLabels.DefaultHeightRatioToChart property {#defaultheightratiotochart}

**Type:** float

### DataLabels.XRatioToChart property {#xratiotochart}

**Type:** float

### DataLabels.YRatioToChart property {#yratiotochart}

**Type:** float

### DataLabels.WidthRatioToChart property {#widthratiotochart}

**Type:** float

### DataLabels.HeightRatioToChart property {#heightratiotochart}

**Type:** float

### DataLabels.XPixel property {#xpixel}

**Type:** int

### DataLabels.YPixel property {#ypixel}

**Type:** int

### DataLabels.WidthPixel property {#widthpixel}

Represents width

**Type:** int

### DataLabels.HeightPixel property {#heightpixel}

Represents height

**Type:** int

### applyFont() {#applyfont}

Apply the font of the datalabels to all child nodes.

### characters(startIndex, length) {#characters}

Returns a Characters object that represents a range of characters within the text.

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int | The index of the start of the character. |
| length | int | The number of characters. |

**Returns:** Characters object.

### setPositionAuto() {#setpositionauto}

Set position of the frame to automatic
