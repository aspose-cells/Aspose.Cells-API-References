---
title: PlotArea
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the object that represents the plot area in a chart.
type: docs
url: /nodejs-cpp/plotarea/
---

## PlotArea class

Encapsulates the object that represents the plot area in a chart.

```javascript
class PlotArea extends ChartFrame;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(ChartFrame)](#constructor-chartframe-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getX()](#getX--)| Gets or gets the x coordinate of the upper left corner of plot-area bounding box in units of 1/4000 of the chart area. |
| [setX(number)](#setX-number-)| Gets or gets the x coordinate of the upper left corner of plot-area bounding box in units of 1/4000 of the chart area. |
| [getY()](#getY--)| Gets or gets the y coordinate of the upper top corner  of plot-area bounding box in units of 1/4000 of the chart area. |
| [setY(number)](#setY-number-)| Gets or gets the y coordinate of the upper top corner  of plot-area bounding box in units of 1/4000 of the chart area. |
| [getHeight()](#getHeight--)| Gets or sets the height of plot-area bounding box in units of 1/4000 of the chart area. |
| [setHeight(number)](#setHeight-number-)| Gets or sets the height of plot-area bounding box in units of 1/4000 of the chart area. |
| [getWidth()](#getWidth--)| Gets or sets the width of plot-area bounding box in units of 1/4000 of the chart area. |
| [setWidth(number)](#setWidth-number-)| Gets or sets the width of plot-area bounding box in units of 1/4000 of the chart area. |
| [getInnerX()](#getInnerX--)| Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. |
| [setInnerX(number)](#setInnerX-number-)| Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. |
| [getInnerY()](#getInnerY--)| Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. |
| [setInnerY(number)](#setInnerY-number-)| Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. |
| [getInnerHeight()](#getInnerHeight--)| Gets or sets the height of plot area in units of 1/4000 of the chart area. |
| [setInnerHeight(number)](#setInnerHeight-number-)| Gets or sets the height of plot area in units of 1/4000 of the chart area. |
| [getInnerWidth()](#getInnerWidth--)| Gets or sets the width  of plot area in units of 1/4000 of the chart area. |
| [setInnerWidth(number)](#setInnerWidth-number-)| Gets or sets the width  of plot area in units of 1/4000 of the chart area. |
| [isAutomaticSize()](#isAutomaticSize--)| Indicates whether the plot area is automatic sized. |
| [setIsAutomaticSize(boolean)](#setIsAutomaticSize-boolean-)| Indicates whether the plot area is automatic sized. |
| [setPositionAuto()](#setPositionAuto--)| Set position of the plot area to automatic |
| [isInnerMode()](#isInnerMode--)| Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [setIsInnerMode(boolean)](#setIsInnerMode-boolean-)| Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [getBackgroundMode()](#getBackgroundMode--)| Gets and sets the display mode of the background |
| [setBackgroundMode(BackgroundMode)](#setBackgroundMode-backgroundmode-)| Gets and sets the display mode of the background |
| [getShadow()](#getShadow--)| True if the frame has a shadow. |
| [setShadow(boolean)](#setShadow-boolean-)| True if the frame has a shadow. |
| [getShapeProperties()](#getShapeProperties--)| Gets the [ShapeProperties](./shapeproperties/) object. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--)| Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [getDefaultX()](#getDefaultX--)| Represents x of default position |
| [getDefaultY()](#getDefaultY--)| Represents y of default position |
| [getDefaultWidth()](#getDefaultWidth--)| Represents width of default position |
| [getDefaultHeight()](#getDefaultHeight--)| Represents height of default position |
| [getBorder()](#getBorder--)| Gets the <see cref="Line">border</see>. |
| [getArea()](#getArea--)| Gets the <see cref="Area">area</see>. |
| [getTextOptions()](#getTextOptions--)| Gets and sets the options of the text. |
| [getFont()](#getFont--)| Gets a [Font](./font/) object of the specified ChartFrame object. |
| [getAutoScaleFont()](#getAutoScaleFont--)| True if the text in the object changes font size when the object size changes. The default value is True. |
| [setAutoScaleFont(boolean)](#setAutoScaleFont-boolean-)| True if the text in the object changes font size when the object size changes. The default value is True. |


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

Gets or gets the x coordinate of the upper left corner of plot-area bounding box in units of 1/4000 of the chart area.

```javascript
getX() : number;
```


**Remarks**

<p>The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerX</b>, <b>InnerY</b>, <b>InnerWidth</b> and <b>InnerHeight</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p>

### setX(number) {#setX-number-}

Gets or gets the x coordinate of the upper left corner of plot-area bounding box in units of 1/4000 of the chart area.

```javascript
setX(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

<p>The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerX</b>, <b>InnerY</b>, <b>InnerWidth</b> and <b>InnerHeight</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p>

### getY() {#getY--}

Gets or gets the y coordinate of the upper top corner  of plot-area bounding box in units of 1/4000 of the chart area.

```javascript
getY() : number;
```


**Remarks**

<p>The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerX</b>, <b>InnerY</b>, <b>InnerWidth</b> and <b>InnerHeight</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p>

### setY(number) {#setY-number-}

Gets or gets the y coordinate of the upper top corner  of plot-area bounding box in units of 1/4000 of the chart area.

```javascript
setY(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

<p>The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerX</b>, <b>InnerY</b>, <b>InnerWidth</b> and <b>InnerHeight</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p>

### getHeight() {#getHeight--}

Gets or sets the height of plot-area bounding box in units of 1/4000 of the chart area.

```javascript
getHeight() : number;
```


**Remarks**

<p>The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerX</b>, <b>InnerY</b>, <b>InnerWidth</b> and <b>InnerHeight</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p>

### setHeight(number) {#setHeight-number-}

Gets or sets the height of plot-area bounding box in units of 1/4000 of the chart area.

```javascript
setHeight(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

<p>The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerX</b>, <b>InnerY</b>, <b>InnerWidth</b> and <b>InnerHeight</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p>

### getWidth() {#getWidth--}

Gets or sets the width of plot-area bounding box in units of 1/4000 of the chart area.

```javascript
getWidth() : number;
```


**Remarks**

<p>The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerX</b>, <b>InnerY</b>, <b>InnerWidth</b> and <b>InnerHeight</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p>

### setWidth(number) {#setWidth-number-}

Gets or sets the width of plot-area bounding box in units of 1/4000 of the chart area.

```javascript
setWidth(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

<p>The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerX</b>, <b>InnerY</b>, <b>InnerWidth</b> and <b>InnerHeight</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p>

### getInnerX() {#getInnerX--}

Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area.

```javascript
getInnerX() : number;
```


**Remarks**

<p>The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerX</b>, <b>InnerY</b>, <b>InnerWidth</b> and <b>InnerHeight</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p>

### setInnerX(number) {#setInnerX-number-}

Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area.

```javascript
setInnerX(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

<p>The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerX</b>, <b>InnerY</b>, <b>InnerWidth</b> and <b>InnerHeight</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p>

### getInnerY() {#getInnerY--}

Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area.

```javascript
getInnerY() : number;
```


**Remarks**

<p>The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerX</b>, <b>InnerY</b>, <b>InnerWidth</b> and <b>InnerHeight</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p>

### setInnerY(number) {#setInnerY-number-}

Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area.

```javascript
setInnerY(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

<p>The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerX</b>, <b>InnerY</b>, <b>InnerWidth</b> and <b>InnerHeight</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p>

### getInnerHeight() {#getInnerHeight--}

Gets or sets the height of plot area in units of 1/4000 of the chart area.

```javascript
getInnerHeight() : number;
```


**Remarks**

<p>The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerX</b>, <b>InnerY</b>, <b>InnerWidth</b> and <b>InnerHeight</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p>

### setInnerHeight(number) {#setInnerHeight-number-}

Gets or sets the height of plot area in units of 1/4000 of the chart area.

```javascript
setInnerHeight(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

<p>The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerX</b>, <b>InnerY</b>, <b>InnerWidth</b> and <b>InnerHeight</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p>

### getInnerWidth() {#getInnerWidth--}

Gets or sets the width  of plot area in units of 1/4000 of the chart area.

```javascript
getInnerWidth() : number;
```


**Remarks**

<p>The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerX</b>, <b>InnerY</b>, <b>InnerWidth</b> and <b>InnerHeight</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p>

### setInnerWidth(number) {#setInnerWidth-number-}

Gets or sets the width  of plot area in units of 1/4000 of the chart area.

```javascript
setInnerWidth(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

<p>The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerX</b>, <b>InnerY</b>, <b>InnerWidth</b> and <b>InnerHeight</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p>

### isAutomaticSize() {#isAutomaticSize--}

Indicates whether the plot area is automatic sized.

```javascript
isAutomaticSize() : boolean;
```


### setIsAutomaticSize(boolean) {#setIsAutomaticSize-boolean-}

Indicates whether the plot area is automatic sized.

```javascript
setIsAutomaticSize(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### setPositionAuto() {#setPositionAuto--}

Set position of the plot area to automatic

```javascript
setPositionAuto() : void;
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

[BackgroundMode](./backgroundmode/)

### setBackgroundMode(BackgroundMode) {#setBackgroundMode-backgroundmode-}

Gets and sets the display mode of the background

```javascript
setBackgroundMode(value: BackgroundMode) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [BackgroundMode](./backgroundmode/) | The value to set. |

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

Gets the [ShapeProperties](./shapeproperties/) object.

```javascript
getShapeProperties() : ShapePropertyCollection;
```


**Returns**

[ShapePropertyCollection](./shapepropertycollection/)

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


### getBorder() {#getBorder--}

Gets the <see cref="Line">border</see>.

```javascript
getBorder() : Line;
```


**Returns**

[Line](./line/)

### getArea() {#getArea--}

Gets the <see cref="Area">area</see>.

```javascript
getArea() : Area;
```


**Returns**

[Area](./area/)

### getTextOptions() {#getTextOptions--}

Gets and sets the options of the text.

```javascript
getTextOptions() : TextOptions;
```


**Returns**

[TextOptions](./textoptions/)

### getFont() {#getFont--}

Gets a [Font](./font/) object of the specified ChartFrame object.

```javascript
getFont() : Font;
```


**Returns**

[Font](./font/)

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


