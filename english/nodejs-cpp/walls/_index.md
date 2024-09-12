---
title: Walls
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the object that represents the walls of a 3D chart.
type: docs
url: /nodejs-cpp/walls/
---

## Walls class

Encapsulates the object that represents the walls of a 3-D chart.

```javascript
class Walls extends Floor;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(Floor)](#constructor-floor-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getCenterX()](#getCenterX--)| Gets the x coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [getCenterY()](#getCenterY--)| Gets the y coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [getWidth()](#getWidth--)| Gets the width of left to right in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [getDepth()](#getDepth--)| Gets the depth front to back in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [getHeight()](#getHeight--)| Gets the height of top to bottom in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [getCenterXPx()](#getCenterXPx--)| Gets the x coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method. |
| [getCenterYPx()](#getCenterYPx--)| Gets the y coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method. |
| [getWidthPx()](#getWidthPx--)| Gets the width of left to right in units of pixels after calls Chart.Calculate() method. |
| [getDepthPx()](#getDepthPx--)| Gets the depth front to back in units of pixels after calls Chart.Calculate() method. |
| [getHeightPx()](#getHeightPx--)| Gets the height of top to bottom in units of pixels after calls Chart.Calculate() method. |
| [getCubePointCount()](#getCubePointCount--)| Gets the number of cube points after calls Chart.Calculate() method. |
| [getCubePointXPx(number)](#getCubePointXPx-number-)| Gets x-coordinate of the apex point of walls cube after calls Chart.Calculate() method. The number of apex points of walls cube is eight |
| [getCubePointYPx(number)](#getCubePointYPx-number-)| Gets y-coordinate of the apex point of walls cube after calls Chart.Calculate() method. The number of apex points of walls cube is eight. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getBackgroundColor()](#getBackgroundColor--)| Gets or sets the background [System.Drawing.Color](../system.drawing.color/) of the [System.Drawing.Color](../system.drawing.color/). |
| [setBackgroundColor(Color)](#setBackgroundColor-color-)| Gets or sets the background [System.Drawing.Color](../system.drawing.color/) of the [System.Drawing.Color](../system.drawing.color/). |
| [getForegroundColor()](#getForegroundColor--)| Gets or sets the foreground [System.Drawing.Color](../system.drawing.color/). |
| [setForegroundColor(Color)](#setForegroundColor-color-)| Gets or sets the foreground [System.Drawing.Color](../system.drawing.color/). |
| [getFormatting()](#getFormatting--)| Represents the formatting of the area. |
| [setFormatting(FormattingType)](#setFormatting-formattingtype-)| Represents the formatting of the area. |
| [getInvertIfNegative()](#getInvertIfNegative--)| If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [setInvertIfNegative(boolean)](#setInvertIfNegative-boolean-)| If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [getFillFormat()](#getFillFormat--)| Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape. |
| [getTransparency()](#getTransparency--)| Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTransparency(number)](#setTransparency-number-)| Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [getBorder()](#getBorder--)| Gets or sets the border [Line](../line/). |
| [setBorder(Line)](#setBorder-line-)| Gets or sets the border [Line](../line/). |


### constructor(Floor) {#constructor-floor-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: Floor);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Floor | The parent object. |

### getCenterX() {#getCenterX--}

Gets the x coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's width after calls Chart.Calculate() method.

```javascript
getCenterX() : number;
```


### getCenterY() {#getCenterY--}

Gets the y coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's height after calls Chart.Calculate() method.

```javascript
getCenterY() : number;
```


### getWidth() {#getWidth--}

Gets the width of left to right in units of 1/4000 of chart's width after calls Chart.Calculate() method.

```javascript
getWidth() : number;
```


### getDepth() {#getDepth--}

Gets the depth front to back in units of 1/4000 of chart's width after calls Chart.Calculate() method.

```javascript
getDepth() : number;
```


### getHeight() {#getHeight--}

Gets the height of top to bottom in units of 1/4000 of chart's height after calls Chart.Calculate() method.

```javascript
getHeight() : number;
```


### getCenterXPx() {#getCenterXPx--}

Gets the x coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method.

```javascript
getCenterXPx() : number;
```


### getCenterYPx() {#getCenterYPx--}

Gets the y coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method.

```javascript
getCenterYPx() : number;
```


### getWidthPx() {#getWidthPx--}

Gets the width of left to right in units of pixels after calls Chart.Calculate() method.

```javascript
getWidthPx() : number;
```


### getDepthPx() {#getDepthPx--}

Gets the depth front to back in units of pixels after calls Chart.Calculate() method.

```javascript
getDepthPx() : number;
```


### getHeightPx() {#getHeightPx--}

Gets the height of top to bottom in units of pixels after calls Chart.Calculate() method.

```javascript
getHeightPx() : number;
```


### getCubePointCount() {#getCubePointCount--}

Gets the number of cube points after calls Chart.Calculate() method.

```javascript
getCubePointCount() : number;
```


### getCubePointXPx(number) {#getCubePointXPx-number-}

Gets x-coordinate of the apex point of walls cube after calls Chart.Calculate() method. The number of apex points of walls cube is eight

```javascript
getCubePointXPx(index: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |

### getCubePointYPx(number) {#getCubePointYPx-number-}

Gets y-coordinate of the apex point of walls cube after calls Chart.Calculate() method. The number of apex points of walls cube is eight.

```javascript
getCubePointYPx(index: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### getBackgroundColor() {#getBackgroundColor--}

Gets or sets the background [System.Drawing.Color](../system.drawing.color/) of the [System.Drawing.Color](../system.drawing.color/).

```javascript
getBackgroundColor() : Color;
```


**Returns**

[Color](../color/)

### setBackgroundColor(Color) {#setBackgroundColor-color-}

Gets or sets the background [System.Drawing.Color](../system.drawing.color/) of the [System.Drawing.Color](../system.drawing.color/).

```javascript
setBackgroundColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |

### getForegroundColor() {#getForegroundColor--}

Gets or sets the foreground [System.Drawing.Color](../system.drawing.color/).

```javascript
getForegroundColor() : Color;
```


**Returns**

[Color](../color/)

### setForegroundColor(Color) {#setForegroundColor-color-}

Gets or sets the foreground [System.Drawing.Color](../system.drawing.color/).

```javascript
setForegroundColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |

### getFormatting() {#getFormatting--}

Represents the formatting of the area.

```javascript
getFormatting() : FormattingType;
```


**Returns**

[FormattingType](../formattingtype/)

### setFormatting(FormattingType) {#setFormatting-formattingtype-}

Represents the formatting of the area.

```javascript
setFormatting(value: FormattingType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FormattingType](../formattingtype/) | The value to set. |

### getInvertIfNegative() {#getInvertIfNegative--}

If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```javascript
getInvertIfNegative() : boolean;
```


### setInvertIfNegative(boolean) {#setInvertIfNegative-boolean-}

If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```javascript
setInvertIfNegative(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getFillFormat() {#getFillFormat--}

Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape.

```javascript
getFillFormat() : FillFormat;
```


**Returns**

[FillFormat](../fillformat/)

### getTransparency() {#getTransparency--}

Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

```javascript
getTransparency() : number;
```


### setTransparency(number) {#setTransparency-number-}

Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

```javascript
setTransparency(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getBorder() {#getBorder--}

Gets or sets the border [Line](../line/).

```javascript
getBorder() : Line;
```


**Returns**

[Line](../line/)

### setBorder(Line) {#setBorder-line-}

Gets or sets the border [Line](../line/).

```javascript
setBorder(value: Line) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Line](../line/) | The value to set. |


