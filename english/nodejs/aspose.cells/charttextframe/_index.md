---
title: "ChartTextFrame"
linktitle: "ChartTextFrame"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Encapsulates the object that represents the frame object which contains text."
type: docs
weight: 590
url: /nodejs/aspose.cells/charttextframe/
---

## ChartTextFrame class

Encapsulates the object that represents the frame object which contains text.

## Methods

| Name | Description |
| --- | --- |
| [characters(startIndex, length)](#characters) | Returns a Characters object that represents a range of characters within the text. |
| [getArea()](#getarea) | Gets the area. |
| [getAutoScaleFont()](#getautoscalefont) | True if the text in the object changes font size when the object size changes. The default value is True. |
| [getBackground()](#getbackground) | Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant.NOTE: This |
| [getBackgroundMode()](#getbackgroundmode) | Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant. |
| [getBorder()](#getborder) | Gets the Line. |
| [getChart()](#getchart) | Gets the chart to which this object belongs. |
| [getDefaultHeight()](#getdefaultheight) | Represents height of default position |
| [getDefaultHeightRatioToChart()](#getdefaultheightratiotochart) |  |
| [getDefaultWidth()](#getdefaultwidth) | Represents width of default position |
| [getDefaultWidthRatioToChart()](#getdefaultwidthratiotochart) |  |
| [getDefaultX()](#getdefaultx) | Represents x of default position |
| [getDefaultXRatioToChart()](#getdefaultxratiotochart) |  |
| [getDefaultY()](#getdefaulty) | Represents y of default position |
| [getDefaultYRatioToChart()](#getdefaultyratiotochart) |  |
| [getDirectionType()](#getdirectiontype) | Gets and sets the direction of text. The value of the property is ChartTextDirectionType integer constant. |
| [getFont()](#getfont) | Gets a Font object of the specified ChartFrame object. |
| [getHeight()](#getheight) | Gets or sets the height of frame in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Height  |
| [getHeightPixel()](#getheightpixel) | Represents height |
| [getHeightRatioToChart()](#getheightratiotochart) |  |
| [getLinkedSource()](#getlinkedsource) | Gets and sets a reference to the worksheet. |
| [getReadingOrder()](#getreadingorder) | Represents text reading order. The value of the property is TextDirectionType integer constant. |
| [getRotationAngle()](#getrotationangle) | Represents text rotation angle. 0: Not rotated.255: Top to Bottom.-90: Downward.90: Upward. |
| [getShadow()](#getshadow) | True if the frame has a shadow. |
| [getShapeProperties()](#getshapeproperties) | Gets the ShapeProperties object. |
| [getText()](#gettext) | Gets or sets the text of a frame's title. |
| [getTextDirection()](#gettextdirection) | Represents text reading order. The value of the property is TextDirectionType integer constant.NOTE: This member is now  |
| [getTextFont()](#gettextfont) | Gets a Font object of the specified ChartFrame object. NOTE: This member is now obsolete. Instead, please use ChartFrame |
| [getTextHorizontalAlignment()](#gettexthorizontalalignment) | Gets and sets the text horizontal alignment. The value of the property is TextAlignmentType integer constant. |
| [getTextOptions()](#gettextoptions) | Gets and sets the options of the text. |
| [getTextVerticalAlignment()](#gettextverticalalignment) | Gets or sets the text vertical alignment of text. The value of the property is TextAlignmentType integer constant. |
| [getWidth()](#getwidth) | Gets or sets the width of frame in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Width In |
| [getWidthPixel()](#getwidthpixel) | Represents width |
| [getWidthRatioToChart()](#getwidthratiotochart) |  |
| [getX()](#getx) | Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. How to convert units of 1/4 |
| [getXPixel()](#getxpixel) |  |
| [getXRatioToChart()](#getxratiotochart) |  |
| [getY()](#gety) | Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. How to convert units of 1/4 |
| [getYPixel()](#getypixel) |  |
| [getYRatioToChart()](#getyratiotochart) |  |
| [isAutoText()](#isautotext) | Indicates the text is auto generated. |
| [isAutomaticRotation()](#isautomaticrotation) | Indicates whether the text of the chart is automatically rotated. |
| [isAutomaticSize()](#isautomaticsize) | Indicates whether the chart frame is automatic sized. |
| [isDefaultPosBeSet()](#isdefaultposbeset) | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [isDeleted()](#isdeleted) | Indicates whether this data labels is deleted. |
| [isInnerMode()](#isinnermode) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the  |
| [isResizeShapeToFitText()](#isresizeshapetofittext) | Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text |
| [isTextWrapped()](#istextwrapped) | Gets or sets a value indicating whether the text is wrapped. |
| [setAutoScaleFont()](#setautoscalefont) | True if the text in the object changes font size when the object size changes. The default value is True. |
| [setAutoText()](#setautotext) | Indicates the text is auto generated. |
| [setAutomaticSize()](#setautomaticsize) | Indicates whether the chart frame is automatic sized. |
| [setBackground()](#setbackground) | Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant.NOTE: This |
| [setBackgroundMode()](#setbackgroundmode) | Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant. |
| [setDeleted()](#setdeleted) | Indicates whether this data labels is deleted. |
| [setDirectionType()](#setdirectiontype) | Gets and sets the direction of text. The value of the property is ChartTextDirectionType integer constant. |
| [setHeight()](#setheight) | Gets or sets the height of frame in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Height  |
| [setHeightPixel()](#setheightpixel) | Represents height |
| [setHeightRatioToChart()](#setheightratiotochart) |  |
| [setInnerMode()](#setinnermode) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the  |
| [setLinkedSource()](#setlinkedsource) | Gets and sets a reference to the worksheet. |
| [setPositionAuto()](#setpositionauto) | Set position of the frame to automatic |
| [setReadingOrder()](#setreadingorder) | Represents text reading order. The value of the property is TextDirectionType integer constant. |
| [setResizeShapeToFitText()](#setresizeshapetofittext) | Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text |
| [setRotationAngle()](#setrotationangle) | Represents text rotation angle. 0: Not rotated.255: Top to Bottom.-90: Downward.90: Upward. |
| [setShadow()](#setshadow) | True if the frame has a shadow. |
| [setText()](#settext) | Gets or sets the text of a frame's title. |
| [setTextDirection()](#settextdirection) | Represents text reading order. The value of the property is TextDirectionType integer constant.NOTE: This member is now  |
| [setTextHorizontalAlignment()](#settexthorizontalalignment) | Gets and sets the text horizontal alignment. The value of the property is TextAlignmentType integer constant. |
| [setTextVerticalAlignment()](#settextverticalalignment) | Gets or sets the text vertical alignment of text. The value of the property is TextAlignmentType integer constant. |
| [setTextWrapped()](#settextwrapped) | Gets or sets a value indicating whether the text is wrapped. |
| [setWidth()](#setwidth) | Gets or sets the width of frame in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Width In |
| [setWidthPixel()](#setwidthpixel) | Represents width |
| [setWidthRatioToChart()](#setwidthratiotochart) |  |
| [setX()](#setx) | Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. How to convert units of 1/4 |
| [setXPixel()](#setxpixel) |  |
| [setXRatioToChart()](#setxratiotochart) |  |
| [setY()](#sety) | Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. How to convert units of 1/4 |
| [setYPixel()](#setypixel) |  |
| [setYRatioToChart()](#setyratiotochart) |  |

### characters(startIndex, length) {#characters}

Returns a Characters object that represents a range of characters within the text.

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Number | The index of the start of the character. |
| length | Number | The number of characters. |

**Returns:** FontSetting — `FontSetting` Characters object.

### getArea() {#getarea}

Gets the area.

### getAutoScaleFont() {#getautoscalefont}

True if the text in the object changes font size when the object size changes. The default value is True.

### getBackground() {#getbackground}

Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant.NOTE: This member is now obsolete. Instead, please use ChartFrame.BackgroundMode property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

### getBackgroundMode() {#getbackgroundmode}

Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant.

### getBorder() {#getborder}

Gets the Line.

### getChart() {#getchart}

Gets the chart to which this object belongs.

### getDefaultHeight() {#getdefaultheight}

Represents height of default position

### getDefaultHeightRatioToChart() {#getdefaultheightratiotochart}

### getDefaultWidth() {#getdefaultwidth}

Represents width of default position

### getDefaultWidthRatioToChart() {#getdefaultwidthratiotochart}

### getDefaultX() {#getdefaultx}

Represents x of default position

### getDefaultXRatioToChart() {#getdefaultxratiotochart}

### getDefaultY() {#getdefaulty}

Represents y of default position

### getDefaultYRatioToChart() {#getdefaultyratiotochart}

### getDirectionType() {#getdirectiontype}

Gets and sets the direction of text. The value of the property is ChartTextDirectionType integer constant.

### getFont() {#getfont}

Gets a Font object of the specified ChartFrame object.

### getHeight() {#getheight}

Gets or sets the height of frame in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Height In Pixels = Y * Chart.ChartObject.Height / 4000;

### getHeightPixel() {#getheightpixel}

Represents height

### getHeightRatioToChart() {#getheightratiotochart}

### getLinkedSource() {#getlinkedsource}

Gets and sets a reference to the worksheet.

### getReadingOrder() {#getreadingorder}

Represents text reading order. The value of the property is TextDirectionType integer constant.

### getRotationAngle() {#getrotationangle}

Represents text rotation angle. 0: Not rotated.255: Top to Bottom.-90: Downward.90: Upward.

### getShadow() {#getshadow}

True if the frame has a shadow.

### getShapeProperties() {#getshapeproperties}

Gets the ShapeProperties object.

### getText() {#gettext}

Gets or sets the text of a frame's title.

### getTextDirection() {#gettextdirection}

Represents text reading order. The value of the property is TextDirectionType integer constant.NOTE: This member is now obsolete. Instead, please use ChartTextFrame.ReadingOrder property. This property will be removed 12 months later since March 2020. Aspose apologizes for any inconvenience you may have experienced.

### getTextFont() {#gettextfont}

Gets a Font object of the specified ChartFrame object. NOTE: This member is now obsolete. Instead, please use ChartFrame.Font property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

### getTextHorizontalAlignment() {#gettexthorizontalalignment}

Gets and sets the text horizontal alignment. The value of the property is TextAlignmentType integer constant.

### getTextOptions() {#gettextoptions}

Gets and sets the options of the text.

### getTextVerticalAlignment() {#gettextverticalalignment}

Gets or sets the text vertical alignment of text. The value of the property is TextAlignmentType integer constant.

### getWidth() {#getwidth}

Gets or sets the width of frame in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Width In Pixels = Width * Chart.ChartObject.Height / 4000;

### getWidthPixel() {#getwidthpixel}

Represents width

### getWidthRatioToChart() {#getwidthratiotochart}

### getX() {#getx}

Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? X In Pixels = X * Chart.ChartObject.Width / 4000;

### getXPixel() {#getxpixel}

### getXRatioToChart() {#getxratiotochart}

### getY() {#gety}

Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Y In Pixels = Y * Chart.ChartObject.Height / 4000;

### getYPixel() {#getypixel}

### getYRatioToChart() {#getyratiotochart}

### isAutoText() {#isautotext}

Indicates the text is auto generated.

### isAutomaticRotation() {#isautomaticrotation}

Indicates whether the text of the chart is automatically rotated.

### isAutomaticSize() {#isautomaticsize}

Indicates whether the chart frame is automatic sized.

### isDefaultPosBeSet() {#isdefaultposbeset}

Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set.

### isDeleted() {#isdeleted}

Indicates whether this data labels is deleted.

### isInnerMode() {#isinnermode}

Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. Only for Xlsx file.

### isResizeShapeToFitText() {#isresizeshapetofittext}

Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside.

### isTextWrapped() {#istextwrapped}

Gets or sets a value indicating whether the text is wrapped.

### setAutoScaleFont() {#setautoscalefont}

True if the text in the object changes font size when the object size changes. The default value is True.

### setAutoText() {#setautotext}

Indicates the text is auto generated.

### setAutomaticSize() {#setautomaticsize}

Indicates whether the chart frame is automatic sized.

### setBackground() {#setbackground}

Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant.NOTE: This member is now obsolete. Instead, please use ChartFrame.BackgroundMode property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

### setBackgroundMode() {#setbackgroundmode}

Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant.

### setDeleted() {#setdeleted}

Indicates whether this data labels is deleted.

### setDirectionType() {#setdirectiontype}

Gets and sets the direction of text. The value of the property is ChartTextDirectionType integer constant.

### setHeight() {#setheight}

Gets or sets the height of frame in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Height In Pixels = Y * Chart.ChartObject.Height / 4000;

### setHeightPixel() {#setheightpixel}

Represents height

### setHeightRatioToChart() {#setheightratiotochart}

### setInnerMode() {#setinnermode}

Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. Only for Xlsx file.

### setLinkedSource() {#setlinkedsource}

Gets and sets a reference to the worksheet.

### setPositionAuto() {#setpositionauto}

Set position of the frame to automatic

### setReadingOrder() {#setreadingorder}

Represents text reading order. The value of the property is TextDirectionType integer constant.

### setResizeShapeToFitText() {#setresizeshapetofittext}

Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside.

### setRotationAngle() {#setrotationangle}

Represents text rotation angle. 0: Not rotated.255: Top to Bottom.-90: Downward.90: Upward.

### setShadow() {#setshadow}

True if the frame has a shadow.

### setText() {#settext}

Gets or sets the text of a frame's title.

### setTextDirection() {#settextdirection}

Represents text reading order. The value of the property is TextDirectionType integer constant.NOTE: This member is now obsolete. Instead, please use ChartTextFrame.ReadingOrder property. This property will be removed 12 months later since March 2020. Aspose apologizes for any inconvenience you may have experienced.

### setTextHorizontalAlignment() {#settexthorizontalalignment}

Gets and sets the text horizontal alignment. The value of the property is TextAlignmentType integer constant.

### setTextVerticalAlignment() {#settextverticalalignment}

Gets or sets the text vertical alignment of text. The value of the property is TextAlignmentType integer constant.

### setTextWrapped() {#settextwrapped}

Gets or sets a value indicating whether the text is wrapped.

### setWidth() {#setwidth}

Gets or sets the width of frame in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Width In Pixels = Width * Chart.ChartObject.Height / 4000;

### setWidthPixel() {#setwidthpixel}

Represents width

### setWidthRatioToChart() {#setwidthratiotochart}

### setX() {#setx}

Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? X In Pixels = X * Chart.ChartObject.Width / 4000;

### setXPixel() {#setxpixel}

### setXRatioToChart() {#setxratiotochart}

### setY() {#sety}

Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Y In Pixels = Y * Chart.ChartObject.Height / 4000;

### setYPixel() {#setypixel}

### setYRatioToChart() {#setyratiotochart}
