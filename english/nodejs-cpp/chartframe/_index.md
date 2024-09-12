---
title: ChartFrame
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the object that represents the frame object in a chart.
type: docs
url: /nodejs-cpp/chartframe/
---

## ChartFrame class

Encapsulates the object that represents the frame object in a chart.

```javascript
class ChartFrame;
```


## Methods

| Method | Description |
| --- | --- |
| [isInnerMode()](#isInnerMode--)| Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [setIsInnerMode(boolean)](#setIsInnerMode-boolean-)| Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [getBackgroundMode()](#getBackgroundMode--)| Gets and sets the display mode of the background |
| [setBackgroundMode(BackgroundMode)](#setBackgroundMode-backgroundmode-)| Gets and sets the display mode of the background |
| [getShadow()](#getShadow--)| True if the frame has a shadow. |
| [setShadow(boolean)](#setShadow-boolean-)| True if the frame has a shadow. |
| [getShapeProperties()](#getShapeProperties--)| Gets the [ShapeProperties](../shapeproperties/) object. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--)| Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [getDefaultX()](#getDefaultX--)| Represents x of default position |
| [getDefaultY()](#getDefaultY--)| Represents y of default position |
| [getDefaultWidth()](#getDefaultWidth--)| Represents width of default position |
| [getDefaultHeight()](#getDefaultHeight--)| Represents height of default position |
| [setPositionAuto()](#setPositionAuto--)| Set position of the frame to automatic |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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

Represents x of default position

```javascript
getDefaultX() : number;
```


### getDefaultY() {#getDefaultY--}

Represents y of default position

```javascript
getDefaultY() : number;
```


### getDefaultWidth() {#getDefaultWidth--}

Represents width of default position

```javascript
getDefaultWidth() : number;
```


### getDefaultHeight() {#getDefaultHeight--}

Represents height of default position

```javascript
getDefaultHeight() : number;
```


### setPositionAuto() {#setPositionAuto--}

Set position of the frame to automatic

```javascript
setPositionAuto() : void;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
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

How to convert units of 1/4000 to pixels? X In Pixels = X * Chart.ChartObject.Width / 4000;

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

How to convert units of 1/4000 to pixels? X In Pixels = X * Chart.ChartObject.Width / 4000;

### getY() {#getY--}

Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area.

```javascript
getY() : number;
```


**Remarks**

How to convert units of 1/4000 to pixels? Y In Pixels = Y * Chart.ChartObject.Height / 4000;

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

How to convert units of 1/4000 to pixels? Y In Pixels = Y * Chart.ChartObject.Height / 4000;

### getHeight() {#getHeight--}

Gets or sets the height of frame in units of 1/4000 of the chart area.

```javascript
getHeight() : number;
```


**Remarks**

How to convert units of 1/4000 to pixels? Height In Pixels = Y * Chart.ChartObject.Height / 4000;

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

How to convert units of 1/4000 to pixels? Height In Pixels = Y * Chart.ChartObject.Height / 4000;

### getWidth() {#getWidth--}

Gets or sets the width of frame in units of 1/4000 of the chart area.

```javascript
getWidth() : number;
```


**Remarks**

How to convert units of 1/4000 to pixels? Width In Pixels = Width * Chart.ChartObject.Height / 4000;

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

How to convert units of 1/4000 to pixels? Width In Pixels = Width * Chart.ChartObject.Height / 4000;


