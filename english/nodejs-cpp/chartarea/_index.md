---
title: ChartArea
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the object that represents the chart area in the worksheet.
type: docs
url: /nodejs-cpp/chartarea/
---

## ChartArea class

Encapsulates the object that represents the chart area in the worksheet.

```javascript
class ChartArea extends ChartFrame;
```


### Example
```javascript
const { Workbook, ChartType, Color } = require("aspose.cells.node");

//Instantiating a Workbook object
var workbook = new Workbook();
//Obtaining the reference of the first worksheet
var worksheet = workbook.getWorksheets().get(0);
//Adding a sample value to "A1" cell
worksheet.getCells().get("A1").putValue(50);
//Adding a sample value to "A2" cell
worksheet.getCells().get("A2").putValue(100);
//Adding a sample value to "A3" cell
worksheet.getCells().get("A3").putValue(150);
//Adding a sample value to "B1" cell
worksheet.getCells().get("B1").putValue(60);
//Adding a sample value to "B2" cell
worksheet.getCells().get("B2").putValue(32);
//Adding a sample value to "B3" cell
worksheet.getCells().get("B3").putValue(50);
//Adding a chart to the worksheet
var chartIndex = worksheet.getCharts().add(ChartType.Column, 5, 0, 15, 5);
//Accessing the instance of the newly added chart
var chart = worksheet.getCharts().get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.getNSeries().add("A1:B3", true);
//Getting Chart Area
var chartArea = chart.getChartArea();
//Setting the foreground color of the chart area
chartArea.getArea().setForegroundColor(Color.Yellow);
//Setting Chart Area Shadow
chartArea.setShadow(true);
//Saving the Excel file
workbook.save("output/ChartsChartArea.xls");
```
## Constructors

| Name | Description |
| --- | --- |
| [constructor(ChartFrame)](#constructor-chartframe-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getX()](#getX--)| Gets or gets the horizontal offset from its upper left corner column, in units of 1/4000 of the chart area. |
| [setX(number)](#setX-number-)| Gets or gets the horizontal offset from its upper left corner column, in units of 1/4000 of the chart area. |
| [getY()](#getY--)| Gets or gets the vertical offset from its upper left corner row, in units of 1/4000 of the chart area. |
| [setY(number)](#setY-number-)| Gets or gets the vertical offset from its upper left corner row, in units of 1/4000 of the chart area. |
| [getHeight()](#getHeight--)| Gets or sets the vertical offset from its lower right corner row, in units of 1/4000 of the chart area. |
| [setHeight(number)](#setHeight-number-)| Gets or sets the vertical offset from its lower right corner row, in units of 1/4000 of the chart area. |
| [getWidth()](#getWidth--)| Gets or sets the horizontal offset from its lower right corner column, in units of 1/4000 of the chart area. |
| [setWidth(number)](#setWidth-number-)| Gets or sets the horizontal offset from its lower right corner column, in units of 1/4000 of the chart area. |
| [getXRatioToChart()](#getXRatioToChart--)| Gets or gets the horizontal offset from its upper left corner column, in units of ratio of the chart area. |
| [setXRatioToChart(number)](#setXRatioToChart-number-)| Gets or gets the horizontal offset from its upper left corner column, in units of ratio of the chart area. |
| [getYRatioToChart()](#getYRatioToChart--)| Gets or gets the vertical offset from its upper left corner row, in units of ratio of the chart area. |
| [setYRatioToChart(number)](#setYRatioToChart-number-)| Gets or gets the vertical offset from its upper left corner row, in units of ratio of the chart area. |
| [getHeightRatioToChart()](#getHeightRatioToChart--)| Gets or sets the vertical offset from its lower right corner row, in units of ratio of the chart area. |
| [setHeightRatioToChart(number)](#setHeightRatioToChart-number-)| Gets or sets the vertical offset from its lower right corner row, in units of ratio of the chart area. |
| [getWidthRatioToChart()](#getWidthRatioToChart--)| Gets or sets the horizontal offset from its lower right corner column, in units of ratio of the chart area. |
| [setWidthRatioToChart(number)](#setWidthRatioToChart-number-)| Gets or sets the horizontal offset from its lower right corner column, in units of ratio of the chart area. |
| [getFont()](#getFont--)| Gets a [Font](../font/) object of the specified chartarea object. |
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
| [setPositionAuto()](#setPositionAuto--)| Set position of the frame to automatic |
| [getBorder()](#getBorder--)| Gets the <see cref="Line">border</see>. |
| [getArea()](#getArea--)| Gets the <see cref="Area">area</see>. |
| [getTextOptions()](#getTextOptions--)| Gets and sets the options of the text. |
| [getAutoScaleFont()](#getAutoScaleFont--)| True if the text in the object changes font size when the object size changes. The default value is True. |
| [setAutoScaleFont(boolean)](#setAutoScaleFont-boolean-)| True if the text in the object changes font size when the object size changes. The default value is True. |
| [isAutomaticSize()](#isAutomaticSize--)| Indicates whether the chart frame is automatic sized. |
| [setIsAutomaticSize(boolean)](#setIsAutomaticSize-boolean-)| Indicates whether the chart frame is automatic sized. |
| [getXPixel()](#getXPixel--)| Gets or sets the x coordinate of the upper left corner in units of Pixel. |
| [setXPixel(number)](#setXPixel-number-)| Gets or sets the x coordinate of the upper left corner in units of Pixel. |
| [getYPixel()](#getYPixel--)| Gets or sets the y coordinate of the upper left corner in units of Pixel. |
| [setYPixel(number)](#setYPixel-number-)| Gets or sets the y coordinate of the upper left corner in units of Pixel. |
| [getWidthPixel()](#getWidthPixel--)| Gets or sets the width of frame in units of Pixel. |
| [setWidthPixel(number)](#setWidthPixel-number-)| Gets or sets the width of frame in units of Pixel. |
| [getHeightPixel()](#getHeightPixel--)| Gets or sets the height of frame in units of Pixel. |
| [setHeightPixel(number)](#setHeightPixel-number-)| Gets or sets the height of frame in units of Pixel. |


### constructor(ChartFrame) {#constructor-chartframe-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: ChartFrame);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | ChartFrame | The parent object. |

### getX() {#getX--}

Gets or gets the horizontal offset from its upper left corner column, in units of 1/4000 of the chart area.

```javascript
getX() : number;
```


**Remarks**

NOTE: This member is now obsolete. Please use ChartArea.XRatioToChart property, instead. X = XRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### setX(number) {#setX-number-}

Gets or gets the horizontal offset from its upper left corner column, in units of 1/4000 of the chart area.

```javascript
setX(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

NOTE: This member is now obsolete. Please use ChartArea.XRatioToChart property, instead. X = XRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### getY() {#getY--}

Gets or gets the vertical offset from its upper left corner row, in units of 1/4000 of the chart area.

```javascript
getY() : number;
```


**Remarks**

NOTE: This member is now obsolete. Please use ChartArea.YRatioToChart property, instead. Y = YRatioToChart * 4000; This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### setY(number) {#setY-number-}

Gets or gets the vertical offset from its upper left corner row, in units of 1/4000 of the chart area.

```javascript
setY(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

NOTE: This member is now obsolete. Please use ChartArea.YRatioToChart property, instead. Y = YRatioToChart * 4000; This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### getHeight() {#getHeight--}

Gets or sets the vertical offset from its lower right corner row, in units of 1/4000 of the chart area.

```javascript
getHeight() : number;
```


**Remarks**

NOTE: This member is now obsolete. Please use ChartArea.HeightRatioToChart property, instead. Height = HeightRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### setHeight(number) {#setHeight-number-}

Gets or sets the vertical offset from its lower right corner row, in units of 1/4000 of the chart area.

```javascript
setHeight(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

NOTE: This member is now obsolete. Please use ChartArea.HeightRatioToChart property, instead. Height = HeightRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### getWidth() {#getWidth--}

Gets or sets the horizontal offset from its lower right corner column, in units of 1/4000 of the chart area.

```javascript
getWidth() : number;
```


**Remarks**

NOTE: This member is now obsolete. Please use ChartArea.WidthRatioToChart property, instead. Width = WidthRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### setWidth(number) {#setWidth-number-}

Gets or sets the horizontal offset from its lower right corner column, in units of 1/4000 of the chart area.

```javascript
setWidth(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

NOTE: This member is now obsolete. Please use ChartArea.WidthRatioToChart property, instead. Width = WidthRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### getXRatioToChart() {#getXRatioToChart--}

Gets or gets the horizontal offset from its upper left corner column, in units of ratio of the chart area.

```javascript
getXRatioToChart() : number;
```


### setXRatioToChart(number) {#setXRatioToChart-number-}

Gets or gets the horizontal offset from its upper left corner column, in units of ratio of the chart area.

```javascript
setXRatioToChart(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getYRatioToChart() {#getYRatioToChart--}

Gets or gets the vertical offset from its upper left corner row, in units of ratio of the chart area.

```javascript
getYRatioToChart() : number;
```


### setYRatioToChart(number) {#setYRatioToChart-number-}

Gets or gets the vertical offset from its upper left corner row, in units of ratio of the chart area.

```javascript
setYRatioToChart(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHeightRatioToChart() {#getHeightRatioToChart--}

Gets or sets the vertical offset from its lower right corner row, in units of ratio of the chart area.

```javascript
getHeightRatioToChart() : number;
```


### setHeightRatioToChart(number) {#setHeightRatioToChart-number-}

Gets or sets the vertical offset from its lower right corner row, in units of ratio of the chart area.

```javascript
setHeightRatioToChart(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWidthRatioToChart() {#getWidthRatioToChart--}

Gets or sets the horizontal offset from its lower right corner column, in units of ratio of the chart area.

```javascript
getWidthRatioToChart() : number;
```


### setWidthRatioToChart(number) {#setWidthRatioToChart-number-}

Gets or sets the horizontal offset from its lower right corner column, in units of ratio of the chart area.

```javascript
setWidthRatioToChart(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getFont() {#getFont--}

Gets a [Font](../font/) object of the specified chartarea object.

```javascript
getFont() : Font;
```


**Returns**

[Font](../font/)

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


### setPositionAuto() {#setPositionAuto--}

Set position of the frame to automatic

```javascript
setPositionAuto() : void;
```


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


