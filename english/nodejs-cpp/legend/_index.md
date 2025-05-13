﻿---
title: Legend
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the object that represents the chart legend.
type: docs
url: /nodejs-cpp/legend/
---

## Legend class

Encapsulates the object that represents the chart legend.

```javascript
class Legend extends ChartTextFrame;
```


### Example
```javascript
const { Workbook, ChartType, LegendPositionType } = require("aspose.cells.node");

//Set Legend's width and height
var workbook = new Workbook();
var sheetIndex = workbook.getWorksheets().add();
var worksheet = workbook.getWorksheets().get(sheetIndex);
var charts = worksheet.getCharts();
//Create a chart
var chart = charts.get(charts.add(ChartType.Column, 1, 1, 10, 10));
var legend = chart.getLegend();

//Legend is at right side of chart by default.
//If the legend is at left or right side of the chart, setting Legend.X property will not take effect.
//If the legend is at top or bottom side of the chart, setting Legend.Y property will not take effect.
legend.setY(1500);
legend.setWidth(50);
legend.setHeight(50);
//Set legend's position
legend.setPosition(LegendPositionType.Left);
```
## Constructors

| Name | Description |
| --- | --- |
| [constructor(ChartTextFrame)](#constructor-charttextframe-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getPosition()](#getPosition--)| Gets or sets the legend position type. |
| [setPosition(LegendPositionType)](#setPosition-legendpositiontype-)| Gets or sets the legend position type. |
| [getLegendEntries()](#getLegendEntries--)| Gets a collection of all the LegendEntry objects in the specified chart legend. Setting the legend entries of the surface chart is not supported. So it will return null if the chart type is surface chart type. |
| [isOverLay()](#isOverLay--)| Gets or sets whether showing the legend without overlapping the chart. |
| [setIsOverLay(boolean)](#setIsOverLay-boolean-)| Gets or sets whether showing the legend without overlapping the chart. |
| [getLegendLabels()](#getLegendLabels--)| Gets the labels of the legend entries after call Chart.Calculate() method. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [isInnerMode()](#isInnerMode--)| Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [setIsInnerMode(boolean)](#setIsInnerMode-boolean-)| Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [getBackgroundMode()](#getBackgroundMode--)| Gets and sets the display mode of the background |
| [setBackgroundMode(BackgroundMode)](#setBackgroundMode-backgroundmode-)| Gets and sets the display mode of the background |
| [getShadow()](#getShadow--)| True if the frame has a shadow. |
| [setShadow(boolean)](#setShadow-boolean-)| True if the frame has a shadow. |
| [getShapeProperties()](#getShapeProperties--)| Gets the [ShapeProperties](../shapeproperties/) object. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--)| Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [getDefaultX()](#getDefaultX--)| Represents x of default position in units of 1/4000 of the chart area. |
| [getDefaultY()](#getDefaultY--)| Represents y of default position in units of 1/4000 of the chart area. |
| [getDefaultWidth()](#getDefaultWidth--)| Represents width of default position in units of 1/4000 of the chart area. |
| [getDefaultHeight()](#getDefaultHeight--)| Represents height of default position in units of 1/4000 of the chart area. |
| [getDefaultXRatioToChart()](#getDefaultXRatioToChart--)| Represents x of default position in units of Fraction of the chart area. |
| [getDefaultYRatioToChart()](#getDefaultYRatioToChart--)| Represents y of default position in units of Fraction of the chart area. |
| [getDefaultWidthRatioToChart()](#getDefaultWidthRatioToChart--)| Represents width of default position in units of Fraction of the chart area. |
| [getDefaultHeightRatioToChart()](#getDefaultHeightRatioToChart--)| Represents height of default position in units of Fraction of the chart area. |
| [isDeleted()](#isDeleted--)| Indicates whether this data labels is deleted. |
| [setIsDeleted(boolean)](#setIsDeleted-boolean-)| Indicates whether this data labels is deleted. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--)| Gets and sets the text horizontal alignment. |
| [setTextHorizontalAlignment(TextAlignmentType)](#setTextHorizontalAlignment-textalignmenttype-)| Gets and sets the text horizontal alignment. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--)| Gets or sets the text vertical alignment of text. |
| [setTextVerticalAlignment(TextAlignmentType)](#setTextVerticalAlignment-textalignmenttype-)| Gets or sets the text vertical alignment of text. |
| [getRotationAngle()](#getRotationAngle--)| Represents text rotation angle. |
| [setRotationAngle(number)](#setRotationAngle-number-)| Represents text rotation angle. |
| [isAutomaticRotation()](#isAutomaticRotation--)| Indicates whether the text of the chart is automatically rotated. |
| [getReadingOrder()](#getReadingOrder--)| Represents text reading order. |
| [setReadingOrder(TextDirectionType)](#setReadingOrder-textdirectiontype-)| Represents text reading order. |
| [isResizeShapeToFitText()](#isResizeShapeToFitText--)| Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside. |
| [setIsResizeShapeToFitText(boolean)](#setIsResizeShapeToFitText-boolean-)| Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside. |
| [characters(number, number)](#characters-number-number-)| Returns a Characters object that represents a range of characters within the text. |
| [getBorder()](#getBorder--)| Gets the <see cref="Line">border</see>. |
| [getArea()](#getArea--)| Gets the <see cref="Area">area</see>. |
| [getTextOptions()](#getTextOptions--)| Gets and sets the options of the text. |
| [getFont()](#getFont--)| Gets a [Font](../font/) object of the specified ChartFrame object. |
| [getAutoScaleFont()](#getAutoScaleFont--)| True if the text in the object changes font size when the object size changes. The default value is True. |
| [setAutoScaleFont(boolean)](#setAutoScaleFont-boolean-)| True if the text in the object changes font size when the object size changes. The default value is True. |
| [isAutomaticSize()](#isAutomaticSize--)| Indicates whether the chart frame is automatic sized. |
| [setIsAutomaticSize(boolean)](#setIsAutomaticSize-boolean-)| Indicates whether the chart frame is automatic sized. |
| [getX()](#getX--)| Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [setX(number)](#setX-number-)| Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [getY()](#getY--)| Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [setY(number)](#setY-number-)| Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [getHeight()](#getHeight--)| Gets or sets the height of frame in units of 1/4000 of the chart area. |
| [setHeight(number)](#setHeight-number-)| Gets or sets the height of frame in units of 1/4000 of the chart area. |
| [getWidth()](#getWidth--)| Gets or sets the width of frame in units of 1/4000 of the chart area. |
| [setWidth(number)](#setWidth-number-)| Gets or sets the width of frame in units of 1/4000 of the chart area. |
| [getXRatioToChart()](#getXRatioToChart--)| Gets or sets the x coordinate of the upper left corner in units of ratio of the chart area. |
| [setXRatioToChart(number)](#setXRatioToChart-number-)| Gets or sets the x coordinate of the upper left corner in units of ratio of the chart area. |
| [getYRatioToChart()](#getYRatioToChart--)| Gets or sets the y coordinate of the upper left corner in units of ratio of the chart area. |
| [setYRatioToChart(number)](#setYRatioToChart-number-)| Gets or sets the y coordinate of the upper left corner in units of ratio of the chart area. |
| [getWidthRatioToChart()](#getWidthRatioToChart--)| Gets or sets the width of frame in units of ratio of the chart area. |
| [setWidthRatioToChart(number)](#setWidthRatioToChart-number-)| Gets or sets the width of frame in units of ratio of the chart area. |
| [getHeightRatioToChart()](#getHeightRatioToChart--)| Gets or sets the height of frame in units of ratio of the chart area. |
| [setHeightRatioToChart(number)](#setHeightRatioToChart-number-)| Gets or sets the height of frame in units of ratio of the chart area. |
| [getXPixel()](#getXPixel--)| Gets or sets the x coordinate of the upper left corner in units of Pixel. |
| [setXPixel(number)](#setXPixel-number-)| Gets or sets the x coordinate of the upper left corner in units of Pixel. |
| [getYPixel()](#getYPixel--)| Gets or sets the y coordinate of the upper left corner in units of Pixel. |
| [setYPixel(number)](#setYPixel-number-)| Gets or sets the y coordinate of the upper left corner in units of Pixel. |
| [getWidthPixel()](#getWidthPixel--)| Gets or sets the width of frame in units of Pixel. |
| [setWidthPixel(number)](#setWidthPixel-number-)| Gets or sets the width of frame in units of Pixel. |
| [getHeightPixel()](#getHeightPixel--)| Gets or sets the height of frame in units of Pixel. |
| [setHeightPixel(number)](#setHeightPixel-number-)| Gets or sets the height of frame in units of Pixel. |
| [setPositionAuto()](#setPositionAuto--)| Set position of the frame to automatic |
| [isAutoText()](#isAutoText--)| Indicates the text is auto generated. |
| [setIsAutoText(boolean)](#setIsAutoText-boolean-)| Indicates the text is auto generated. |
| [getText()](#getText--)| Gets or sets the text of a frame's title. |
| [setText(string)](#setText-string-)| Gets or sets the text of a frame's title. |
| [getLinkedSource()](#getLinkedSource--)| Gets and sets a reference to the worksheet. |
| [setLinkedSource(string)](#setLinkedSource-string-)| Gets and sets a reference to the worksheet. |
| [getDirectionType()](#getDirectionType--)| Gets and sets the direction of text. |
| [setDirectionType(ChartTextDirectionType)](#setDirectionType-charttextdirectiontype-)| Gets and sets the direction of text. |
| [isTextWrapped()](#isTextWrapped--)| Gets or sets a value indicating whether the text is wrapped. |
| [setIsTextWrapped(boolean)](#setIsTextWrapped-boolean-)| Gets or sets a value indicating whether the text is wrapped. |


### constructor(ChartTextFrame) {#constructor-charttextframe-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: ChartTextFrame);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | ChartTextFrame | The parent object. |

### getPosition() {#getPosition--}

Gets or sets the legend position type.

```javascript
getPosition() : LegendPositionType;
```


**Returns**

[LegendPositionType](../legendpositiontype/)

**Remarks**

br>Default position is right.</br> <br>If the legend is at left or right side of the chart, setting Legend.X property will not take effect.</br> <br>If the legend is at top or bottom side of the chart, setting Legend.Y property will not take effect.</br

### setPosition(LegendPositionType) {#setPosition-legendpositiontype-}

Gets or sets the legend position type.

```javascript
setPosition(value: LegendPositionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LegendPositionType](../legendpositiontype/) | The value to set. |

**Remarks**

br>Default position is right.</br> <br>If the legend is at left or right side of the chart, setting Legend.X property will not take effect.</br> <br>If the legend is at top or bottom side of the chart, setting Legend.Y property will not take effect.</br

### getLegendEntries() {#getLegendEntries--}

Gets a collection of all the LegendEntry objects in the specified chart legend. Setting the legend entries of the surface chart is not supported. So it will return null if the chart type is surface chart type.

```javascript
getLegendEntries() : LegendEntryCollection;
```


**Returns**

[LegendEntryCollection](../legendentrycollection/)

### isOverLay() {#isOverLay--}

Gets or sets whether showing the legend without overlapping the chart.

```javascript
isOverLay() : boolean;
```


### setIsOverLay(boolean) {#setIsOverLay-boolean-}

Gets or sets whether showing the legend without overlapping the chart.

```javascript
setIsOverLay(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getLegendLabels() {#getLegendLabels--}

Gets the labels of the legend entries after call Chart.Calculate() method.

```javascript
getLegendLabels() : string[];
```


**Returns**

string[]

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### isInnerMode() {#isInnerMode--}

Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels.

```javascript
isInnerMode() : boolean;
```


**Remarks**

Only for Xlsx file.

### setIsInnerMode(boolean) {#setIsInnerMode-boolean-}

Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels.

```javascript
setIsInnerMode(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only for Xlsx file.

### getBackgroundMode() {#getBackgroundMode--}

Gets and sets the display mode of the background

```javascript
getBackgroundMode() : BackgroundMode;
```


**Returns**

[BackgroundMode](../backgroundmode/)

### setBackgroundMode(BackgroundMode) {#setBackgroundMode-backgroundmode-}

Gets and sets the display mode of the background

```javascript
setBackgroundMode(value: BackgroundMode) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [BackgroundMode](../backgroundmode/) | The value to set. |

### getShadow() {#getShadow--}

True if the frame has a shadow.

```javascript
getShadow() : boolean;
```


### setShadow(boolean) {#setShadow-boolean-}

True if the frame has a shadow.

```javascript
setShadow(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShapeProperties() {#getShapeProperties--}

Gets the [ShapeProperties](../shapeproperties/) object.

```javascript
getShapeProperties() : ShapePropertyCollection;
```


**Returns**

[ShapePropertyCollection](../shapepropertycollection/)

### isDefaultPosBeSet() {#isDefaultPosBeSet--}

Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set.

```javascript
isDefaultPosBeSet() : boolean;
```


### getDefaultX() {#getDefaultX--}

Represents x of default position in units of 1/4000 of the chart area.

```javascript
getDefaultX() : number;
```


**Remarks**

NOTE: This member is now obsolete. Please use ChartFrame.DefaultXRatioToChart property, instead. DefaultX = (int)(DefaultXRatioToChart * 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### getDefaultY() {#getDefaultY--}

Represents y of default position in units of 1/4000 of the chart area.

```javascript
getDefaultY() : number;
```


**Remarks**

NOTE: This member is now obsolete. Please use ChartFrame.DefaultYRatioToChart property, instead. DefaultY = (int)(DefaultYRatioToChart * 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### getDefaultWidth() {#getDefaultWidth--}

Represents width of default position in units of 1/4000 of the chart area.

```javascript
getDefaultWidth() : number;
```


**Remarks**

NOTE: This member is now obsolete. Please use ChartFrame.DefaultWidthRatioToChart property, instead. DefaultWidth = (int)(DefaultWidthRatioToChart * 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### getDefaultHeight() {#getDefaultHeight--}

Represents height of default position in units of 1/4000 of the chart area.

```javascript
getDefaultHeight() : number;
```


**Remarks**

NOTE: This member is now obsolete. Please use ChartFrame.DefaultHeightRatioToChart property, instead. DefaultHeight = (int)(DefaultHeightRatioToChart * 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### getDefaultXRatioToChart() {#getDefaultXRatioToChart--}

Represents x of default position in units of Fraction of the chart area.

```javascript
getDefaultXRatioToChart() : number;
```


### getDefaultYRatioToChart() {#getDefaultYRatioToChart--}

Represents y of default position in units of Fraction of the chart area.

```javascript
getDefaultYRatioToChart() : number;
```


### getDefaultWidthRatioToChart() {#getDefaultWidthRatioToChart--}

Represents width of default position in units of Fraction of the chart area.

```javascript
getDefaultWidthRatioToChart() : number;
```


### getDefaultHeightRatioToChart() {#getDefaultHeightRatioToChart--}

Represents height of default position in units of Fraction of the chart area.

```javascript
getDefaultHeightRatioToChart() : number;
```


### isDeleted() {#isDeleted--}

Indicates whether this data labels is deleted.

```javascript
isDeleted() : boolean;
```


### setIsDeleted(boolean) {#setIsDeleted-boolean-}

Indicates whether this data labels is deleted.

```javascript
setIsDeleted(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}

Gets and sets the text horizontal alignment.

```javascript
getTextHorizontalAlignment() : TextAlignmentType;
```


**Returns**

[TextAlignmentType](../textalignmenttype/)

### setTextHorizontalAlignment(TextAlignmentType) {#setTextHorizontalAlignment-textalignmenttype-}

Gets and sets the text horizontal alignment.

```javascript
setTextHorizontalAlignment(value: TextAlignmentType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](../textalignmenttype/) | The value to set. |

### getTextVerticalAlignment() {#getTextVerticalAlignment--}

Gets or sets the text vertical alignment of text.

```javascript
getTextVerticalAlignment() : TextAlignmentType;
```


**Returns**

[TextAlignmentType](../textalignmenttype/)

### setTextVerticalAlignment(TextAlignmentType) {#setTextVerticalAlignment-textalignmenttype-}

Gets or sets the text vertical alignment of text.

```javascript
setTextVerticalAlignment(value: TextAlignmentType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](../textalignmenttype/) | The value to set. |

### getRotationAngle() {#getRotationAngle--}

Represents text rotation angle.

```javascript
getRotationAngle() : number;
```


**Remarks**

br>0: Not rotated.</br> <br>255: Top to Bottom.</br> <br>-90: Downward.</br> <br>90: Upward.</br

### setRotationAngle(number) {#setRotationAngle-number-}

Represents text rotation angle.

```javascript
setRotationAngle(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

br>0: Not rotated.</br> <br>255: Top to Bottom.</br> <br>-90: Downward.</br> <br>90: Upward.</br

### isAutomaticRotation() {#isAutomaticRotation--}

Indicates whether the text of the chart is automatically rotated.

```javascript
isAutomaticRotation() : boolean;
```


### getReadingOrder() {#getReadingOrder--}

Represents text reading order.

```javascript
getReadingOrder() : TextDirectionType;
```


**Returns**

[TextDirectionType](../textdirectiontype/)

### setReadingOrder(TextDirectionType) {#setReadingOrder-textdirectiontype-}

Represents text reading order.

```javascript
setReadingOrder(value: TextDirectionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextDirectionType](../textdirectiontype/) | The value to set. |

### isResizeShapeToFitText() {#isResizeShapeToFitText--}

Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside.

```javascript
isResizeShapeToFitText() : boolean;
```


### setIsResizeShapeToFitText(boolean) {#setIsResizeShapeToFitText-boolean-}

Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside.

```javascript
setIsResizeShapeToFitText(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### characters(number, number) {#characters-number-number-}

Returns a Characters object that represents a range of characters within the text.

```javascript
characters(startIndex: number, length: number) : FontSetting;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | number | The index of the start of the character. |
| length | number | The number of characters. |

**Returns**

Characters object.

### getBorder() {#getBorder--}

Gets the <see cref="Line">border</see>.

```javascript
getBorder() : Line;
```


**Returns**

[Line](../line/)

### getArea() {#getArea--}

Gets the <see cref="Area">area</see>.

```javascript
getArea() : Area;
```


**Returns**

[Area](../area/)

### getTextOptions() {#getTextOptions--}

Gets and sets the options of the text.

```javascript
getTextOptions() : TextOptions;
```


**Returns**

[TextOptions](../textoptions/)

### getFont() {#getFont--}

Gets a [Font](../font/) object of the specified ChartFrame object.

```javascript
getFont() : Font;
```


**Returns**

[Font](../font/)

### getAutoScaleFont() {#getAutoScaleFont--}

True if the text in the object changes font size when the object size changes. The default value is True.

```javascript
getAutoScaleFont() : boolean;
```


### setAutoScaleFont(boolean) {#setAutoScaleFont-boolean-}

True if the text in the object changes font size when the object size changes. The default value is True.

```javascript
setAutoScaleFont(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isAutomaticSize() {#isAutomaticSize--}

Indicates whether the chart frame is automatic sized.

```javascript
isAutomaticSize() : boolean;
```


### setIsAutomaticSize(boolean) {#setIsAutomaticSize-boolean-}

Indicates whether the chart frame is automatic sized.

```javascript
setIsAutomaticSize(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getX() {#getX--}

Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area.

```javascript
getX() : number;
```


**Remarks**

How to convert units of 1/4000 to pixels? X In Pixels = X * Chart.ChartObject.Width / 4000d;

### setX(number) {#setX-number-}

Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area.

```javascript
setX(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

How to convert units of 1/4000 to pixels? X In Pixels = X * Chart.ChartObject.Width / 4000d;

### getY() {#getY--}

Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area.

```javascript
getY() : number;
```


**Remarks**

How to convert units of 1/4000 to pixels? Y In Pixels = Y * Chart.ChartObject.Height / 4000d;

### setY(number) {#setY-number-}

Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area.

```javascript
setY(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

How to convert units of 1/4000 to pixels? Y In Pixels = Y * Chart.ChartObject.Height / 4000d;

### getHeight() {#getHeight--}

Gets or sets the height of frame in units of 1/4000 of the chart area.

```javascript
getHeight() : number;
```


**Remarks**

How to convert units of 1/4000 to pixels? Height In Pixels = Y * Chart.ChartObject.Height / 4000d;

### setHeight(number) {#setHeight-number-}

Gets or sets the height of frame in units of 1/4000 of the chart area.

```javascript
setHeight(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

How to convert units of 1/4000 to pixels? Height In Pixels = Y * Chart.ChartObject.Height / 4000d;

### getWidth() {#getWidth--}

Gets or sets the width of frame in units of 1/4000 of the chart area.

```javascript
getWidth() : number;
```


**Remarks**

How to convert units of 1/4000 to pixels? Width In Pixels = Width * Chart.ChartObject.Height / 4000d;

### setWidth(number) {#setWidth-number-}

Gets or sets the width of frame in units of 1/4000 of the chart area.

```javascript
setWidth(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

How to convert units of 1/4000 to pixels? Width In Pixels = Width * Chart.ChartObject.Height / 4000d;

### getXRatioToChart() {#getXRatioToChart--}

Gets or sets the x coordinate of the upper left corner in units of ratio of the chart area.

```javascript
getXRatioToChart() : number;
```


**Remarks**

This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? XPixel = XRatioToChart * Chart.ChartObject.Width;

### setXRatioToChart(number) {#setXRatioToChart-number-}

Gets or sets the x coordinate of the upper left corner in units of ratio of the chart area.

```javascript
setXRatioToChart(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? XPixel = XRatioToChart * Chart.ChartObject.Width;

### getYRatioToChart() {#getYRatioToChart--}

Gets or sets the y coordinate of the upper left corner in units of ratio of the chart area.

```javascript
getYRatioToChart() : number;
```


**Remarks**

This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? YPixel = YRatioToChart * Chart.ChartObject.Height;

### setYRatioToChart(number) {#setYRatioToChart-number-}

Gets or sets the y coordinate of the upper left corner in units of ratio of the chart area.

```javascript
setYRatioToChart(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? YPixel = YRatioToChart * Chart.ChartObject.Height;

### getWidthRatioToChart() {#getWidthRatioToChart--}

Gets or sets the width of frame in units of ratio of the chart area.

```javascript
getWidthRatioToChart() : number;
```


**Remarks**

This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? WidthPixel = WidthRatioToChart * Chart.ChartObject.Width;

### setWidthRatioToChart(number) {#setWidthRatioToChart-number-}

Gets or sets the width of frame in units of ratio of the chart area.

```javascript
setWidthRatioToChart(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? WidthPixel = WidthRatioToChart * Chart.ChartObject.Width;

### getHeightRatioToChart() {#getHeightRatioToChart--}

Gets or sets the height of frame in units of ratio of the chart area.

```javascript
getHeightRatioToChart() : number;
```


**Remarks**

This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? HeightPixel = HeightRatioToChart * Chart.ChartObject.Height;

### setHeightRatioToChart(number) {#setHeightRatioToChart-number-}

Gets or sets the height of frame in units of ratio of the chart area.

```javascript
setHeightRatioToChart(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? HeightPixel = HeightRatioToChart * Chart.ChartObject.Height;

### getXPixel() {#getXPixel--}

Gets or sets the x coordinate of the upper left corner in units of Pixel.

```javascript
getXPixel() : number;
```


### setXPixel(number) {#setXPixel-number-}

Gets or sets the x coordinate of the upper left corner in units of Pixel.

```javascript
setXPixel(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getYPixel() {#getYPixel--}

Gets or sets the y coordinate of the upper left corner in units of Pixel.

```javascript
getYPixel() : number;
```


### setYPixel(number) {#setYPixel-number-}

Gets or sets the y coordinate of the upper left corner in units of Pixel.

```javascript
setYPixel(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWidthPixel() {#getWidthPixel--}

Gets or sets the width of frame in units of Pixel.

```javascript
getWidthPixel() : number;
```


### setWidthPixel(number) {#setWidthPixel-number-}

Gets or sets the width of frame in units of Pixel.

```javascript
setWidthPixel(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHeightPixel() {#getHeightPixel--}

Gets or sets the height of frame in units of Pixel.

```javascript
getHeightPixel() : number;
```


### setHeightPixel(number) {#setHeightPixel-number-}

Gets or sets the height of frame in units of Pixel.

```javascript
setHeightPixel(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### setPositionAuto() {#setPositionAuto--}

Set position of the frame to automatic

```javascript
setPositionAuto() : void;
```


### isAutoText() {#isAutoText--}

Indicates the text is auto generated.

```javascript
isAutoText() : boolean;
```


### setIsAutoText(boolean) {#setIsAutoText-boolean-}

Indicates the text is auto generated.

```javascript
setIsAutoText(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getText() {#getText--}

Gets or sets the text of a frame's title.

```javascript
getText() : string;
```


### setText(string) {#setText-string-}

Gets or sets the text of a frame's title.

```javascript
setText(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getLinkedSource() {#getLinkedSource--}

Gets and sets a reference to the worksheet.

```javascript
getLinkedSource() : string;
```


### setLinkedSource(string) {#setLinkedSource-string-}

Gets and sets a reference to the worksheet.

```javascript
setLinkedSource(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getDirectionType() {#getDirectionType--}

Gets and sets the direction of text.

```javascript
getDirectionType() : ChartTextDirectionType;
```


**Returns**

[ChartTextDirectionType](../charttextdirectiontype/)

### setDirectionType(ChartTextDirectionType) {#setDirectionType-charttextdirectiontype-}

Gets and sets the direction of text.

```javascript
setDirectionType(value: ChartTextDirectionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ChartTextDirectionType](../charttextdirectiontype/) | The value to set. |

### isTextWrapped() {#isTextWrapped--}

Gets or sets a value indicating whether the text is wrapped.

```javascript
isTextWrapped() : boolean;
```


### setIsTextWrapped(boolean) {#setIsTextWrapped-boolean-}

Gets or sets a value indicating whether the text is wrapped.

```javascript
setIsTextWrapped(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |


