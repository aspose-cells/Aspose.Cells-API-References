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

| Constructor | Description |
| --- | --- |
| [constructor(ChartFrame)](#constructor-chartframe-)| Constructs from a parent object convertible to this. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [innerX](#innerX--)| number | Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. |
| [innerY](#innerY--)| number | Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. |
| [innerHeight](#innerHeight--)| number | Gets or sets the height of plot area in units of 1/4000 of the chart area. |
| [innerWidth](#innerWidth--)| number | Gets or sets the width  of plot area in units of 1/4000 of the chart area. |
| [innerXRatioToChart](#innerXRatioToChart--)| number | Gets or gets the x coordinate of the upper top corner of plot area in units of ratio of the chart area. |
| [innerYRatioToChart](#innerYRatioToChart--)| number | Gets or gets the x coordinate of the upper top corner of plot area in units of ratio of the chart area. |
| [innerHeightRatioToChart](#innerHeightRatioToChart--)| number | Gets or sets the height of plot area in units of ratio of the chart area. |
| [innerWidthRatioToChart](#innerWidthRatioToChart--)| number | Gets or sets the width  of plot area in units of ratio of the chart area. |
| [isInnerMode](#isInnerMode--)| boolean | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [backgroundMode](#backgroundMode--)| BackgroundMode | Gets and sets the display mode of the background |
| [shadow](#shadow--)| boolean | True if the frame has a shadow. |
| [shapeProperties](#shapeProperties--)| ShapePropertyCollection | Readonly. Gets the [ShapeProperties](../shapeproperties/) object. |
| [isDefaultPosBeSet](#isDefaultPosBeSet--)| boolean | Readonly. Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [defaultX](#defaultX--)| number | Readonly. Represents x of default position in units of 1/4000 of the chart area. |
| [defaultY](#defaultY--)| number | Readonly. Represents y of default position in units of 1/4000 of the chart area. |
| [defaultWidth](#defaultWidth--)| number | Readonly. Represents width of default position in units of 1/4000 of the chart area. |
| [defaultHeight](#defaultHeight--)| number | Readonly. Represents height of default position in units of 1/4000 of the chart area. |
| [defaultXRatioToChart](#defaultXRatioToChart--)| number | Readonly. Represents x of default position in units of Fraction of the chart area. |
| [defaultYRatioToChart](#defaultYRatioToChart--)| number | Readonly. Represents y of default position in units of Fraction of the chart area. |
| [defaultWidthRatioToChart](#defaultWidthRatioToChart--)| number | Readonly. Represents width of default position in units of Fraction of the chart area. |
| [defaultHeightRatioToChart](#defaultHeightRatioToChart--)| number | Readonly. Represents height of default position in units of Fraction of the chart area. |

## Methods

| Method | Description |
| --- | --- |
| [getInnerX()](#getInnerX--)| <b>@deprecated.</b> Please use the 'innerX' property instead. Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. |
| [setInnerX(number)](#setInnerX-number-)| <b>@deprecated.</b> Please use the 'innerX' property instead. Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. |
| [getInnerY()](#getInnerY--)| <b>@deprecated.</b> Please use the 'innerY' property instead. Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. |
| [setInnerY(number)](#setInnerY-number-)| <b>@deprecated.</b> Please use the 'innerY' property instead. Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. |
| [getInnerHeight()](#getInnerHeight--)| <b>@deprecated.</b> Please use the 'innerHeight' property instead. Gets or sets the height of plot area in units of 1/4000 of the chart area. |
| [setInnerHeight(number)](#setInnerHeight-number-)| <b>@deprecated.</b> Please use the 'innerHeight' property instead. Gets or sets the height of plot area in units of 1/4000 of the chart area. |
| [getInnerWidth()](#getInnerWidth--)| <b>@deprecated.</b> Please use the 'innerWidth' property instead. Gets or sets the width  of plot area in units of 1/4000 of the chart area. |
| [setInnerWidth(number)](#setInnerWidth-number-)| <b>@deprecated.</b> Please use the 'innerWidth' property instead. Gets or sets the width  of plot area in units of 1/4000 of the chart area. |
| [getInnerXRatioToChart()](#getInnerXRatioToChart--)| <b>@deprecated.</b> Please use the 'innerXRatioToChart' property instead. Gets or gets the x coordinate of the upper top corner of plot area in units of ratio of the chart area. |
| [setInnerXRatioToChart(number)](#setInnerXRatioToChart-number-)| <b>@deprecated.</b> Please use the 'innerXRatioToChart' property instead. Gets or gets the x coordinate of the upper top corner of plot area in units of ratio of the chart area. |
| [getInnerYRatioToChart()](#getInnerYRatioToChart--)| <b>@deprecated.</b> Please use the 'innerYRatioToChart' property instead. Gets or gets the x coordinate of the upper top corner of plot area in units of ratio of the chart area. |
| [setInnerYRatioToChart(number)](#setInnerYRatioToChart-number-)| <b>@deprecated.</b> Please use the 'innerYRatioToChart' property instead. Gets or gets the x coordinate of the upper top corner of plot area in units of ratio of the chart area. |
| [getInnerHeightRatioToChart()](#getInnerHeightRatioToChart--)| <b>@deprecated.</b> Please use the 'innerHeightRatioToChart' property instead. Gets or sets the height of plot area in units of ratio of the chart area. |
| [setInnerHeightRatioToChart(number)](#setInnerHeightRatioToChart-number-)| <b>@deprecated.</b> Please use the 'innerHeightRatioToChart' property instead. Gets or sets the height of plot area in units of ratio of the chart area. |
| [getInnerWidthRatioToChart()](#getInnerWidthRatioToChart--)| <b>@deprecated.</b> Please use the 'innerWidthRatioToChart' property instead. Gets or sets the width  of plot area in units of ratio of the chart area. |
| [setInnerWidthRatioToChart(number)](#setInnerWidthRatioToChart-number-)| <b>@deprecated.</b> Please use the 'innerWidthRatioToChart' property instead. Gets or sets the width  of plot area in units of ratio of the chart area. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [isInnerMode()](#isInnerMode--)| <b>@deprecated.</b> Please use the 'isInnerMode' property instead. Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [setIsInnerMode(boolean)](#setIsInnerMode-boolean-)| <b>@deprecated.</b> Please use the 'isInnerMode' property instead. Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [getBackgroundMode()](#getBackgroundMode--)| <b>@deprecated.</b> Please use the 'backgroundMode' property instead. Gets and sets the display mode of the background |
| [setBackgroundMode(BackgroundMode)](#setBackgroundMode-backgroundmode-)| <b>@deprecated.</b> Please use the 'backgroundMode' property instead. Gets and sets the display mode of the background |
| [getShadow()](#getShadow--)| <b>@deprecated.</b> Please use the 'shadow' property instead. True if the frame has a shadow. |
| [setShadow(boolean)](#setShadow-boolean-)| <b>@deprecated.</b> Please use the 'shadow' property instead. True if the frame has a shadow. |
| [getShapeProperties()](#getShapeProperties--)| <b>@deprecated.</b> Please use the 'shapeProperties' property instead. Gets the [ShapeProperties](../shapeproperties/) object. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--)| <b>@deprecated.</b> Please use the 'isDefaultPosBeSet' property instead. Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [getDefaultX()](#getDefaultX--)| <b>@deprecated.</b> Please use the 'defaultX' property instead. Represents x of default position in units of 1/4000 of the chart area. |
| [getDefaultY()](#getDefaultY--)| <b>@deprecated.</b> Please use the 'defaultY' property instead. Represents y of default position in units of 1/4000 of the chart area. |
| [getDefaultWidth()](#getDefaultWidth--)| <b>@deprecated.</b> Please use the 'defaultWidth' property instead. Represents width of default position in units of 1/4000 of the chart area. |
| [getDefaultHeight()](#getDefaultHeight--)| <b>@deprecated.</b> Please use the 'defaultHeight' property instead. Represents height of default position in units of 1/4000 of the chart area. |
| [getDefaultXRatioToChart()](#getDefaultXRatioToChart--)| <b>@deprecated.</b> Please use the 'defaultXRatioToChart' property instead. Represents x of default position in units of Fraction of the chart area. |
| [getDefaultYRatioToChart()](#getDefaultYRatioToChart--)| <b>@deprecated.</b> Please use the 'defaultYRatioToChart' property instead. Represents y of default position in units of Fraction of the chart area. |
| [getDefaultWidthRatioToChart()](#getDefaultWidthRatioToChart--)| <b>@deprecated.</b> Please use the 'defaultWidthRatioToChart' property instead. Represents width of default position in units of Fraction of the chart area. |
| [getDefaultHeightRatioToChart()](#getDefaultHeightRatioToChart--)| <b>@deprecated.</b> Please use the 'defaultHeightRatioToChart' property instead. Represents height of default position in units of Fraction of the chart area. |
| [getX()](#getX--)| Gets or gets the x coordinate of the upper left corner of plot-area bounding box in units of 1/4000 of the chart area. |
| [setX(number)](#setX-number-)| Gets or gets the x coordinate of the upper left corner of plot-area bounding box in units of 1/4000 of the chart area. |
| [getY()](#getY--)| Gets or gets the y coordinate of the upper top corner  of plot-area bounding box in units of 1/4000 of the chart area. |
| [setY(number)](#setY-number-)| Gets or gets the y coordinate of the upper top corner  of plot-area bounding box in units of 1/4000 of the chart area. |
| [getHeight()](#getHeight--)| Gets or sets the height of plot-area bounding box in units of 1/4000 of the chart area. |
| [setHeight(number)](#setHeight-number-)| Gets or sets the height of plot-area bounding box in units of 1/4000 of the chart area. |
| [getWidth()](#getWidth--)| Gets or sets the width of plot-area bounding box in units of 1/4000 of the chart area. |
| [setWidth(number)](#setWidth-number-)| Gets or sets the width of plot-area bounding box in units of 1/4000 of the chart area. |
| [getXRatioToChart()](#getXRatioToChart--)| Gets or gets the x coordinate of the upper left corner of plot-area bounding box in units of ratio of the chart area. |
| [setXRatioToChart(number)](#setXRatioToChart-number-)| Gets or gets the x coordinate of the upper left corner of plot-area bounding box in units of ratio of the chart area. |
| [getYRatioToChart()](#getYRatioToChart--)| Gets or gets the y coordinate of the upper top corner  of plot-area bounding box in units of ratio of the chart area. |
| [setYRatioToChart(number)](#setYRatioToChart-number-)| Gets or gets the y coordinate of the upper top corner  of plot-area bounding box in units of ratio of the chart area. |
| [getHeightRatioToChart()](#getHeightRatioToChart--)| Gets or sets the height of plot-area bounding box in units of ratio of the chart area. |
| [setHeightRatioToChart(number)](#setHeightRatioToChart-number-)| Gets or sets the height of plot-area bounding box in units of ratio of the chart area. |
| [getWidthRatioToChart()](#getWidthRatioToChart--)| Gets or sets the width of plot-area bounding box in units of ratio of the chart area. |
| [setWidthRatioToChart(number)](#setWidthRatioToChart-number-)| Gets or sets the width of plot-area bounding box in units of ratio of the chart area. |
| [isAutomaticSize()](#isAutomaticSize--)| Indicates whether the plot area is automatic sized. |
| [setIsAutomaticSize(boolean)](#setIsAutomaticSize-boolean-)| Indicates whether the plot area is automatic sized. |
| [setPositionAuto()](#setPositionAuto--)| Set position of the plot area to automatic |
| [getBorder()](#getBorder--)| Gets the <see cref="Line">border</see>. |
| [getArea()](#getArea--)| Gets the <see cref="Area">area</see>. |
| [getTextOptions()](#getTextOptions--)| Gets and sets the options of the text. |
| [getFont()](#getFont--)| Gets a [Font](../font/) object of the specified ChartFrame object. |
| [getAutoScaleFont()](#getAutoScaleFont--)| True if the text in the object changes font size when the object size changes. The default value is True. |
| [setAutoScaleFont(boolean)](#setAutoScaleFont-boolean-)| True if the text in the object changes font size when the object size changes. The default value is True. |
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

### innerX {#innerX--}

Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area.

```javascript
innerX : number;
```


**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> Note: When InnerX is set, the IsInnerMode property will be automatically set to True.

### innerY {#innerY--}

Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area.

```javascript
innerY : number;
```


**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> Note: When InnerY is set, the IsInnerMode property will be automatically set to True.

### innerHeight {#innerHeight--}

Gets or sets the height of plot area in units of 1/4000 of the chart area.

```javascript
innerHeight : number;
```


**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> Note: When InnerHeight is set, the IsInnerMode property will be automatically set to True.

### innerWidth {#innerWidth--}

Gets or sets the width  of plot area in units of 1/4000 of the chart area.

```javascript
innerWidth : number;
```


**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> Note: When InnerWidth is set, the IsInnerMode property will be automatically set to True.

### innerXRatioToChart {#innerXRatioToChart--}

Gets or gets the x coordinate of the upper top corner of plot area in units of ratio of the chart area.

```javascript
innerXRatioToChart : number;
```


**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>XRatioToChart</b>, <b>YRatioToChart</b>, <b>WidthRatioToChart</b> and <b>HeightRatioToChart</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> InnerX in Pixel = InnerXRatioToChart * chart.ChartObject.Width. Note: When InnerXRatioToChart is set, the IsInnerMode property will be automatically set to True.

### innerYRatioToChart {#innerYRatioToChart--}

Gets or gets the x coordinate of the upper top corner of plot area in units of ratio of the chart area.

```javascript
innerYRatioToChart : number;
```


**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>XRatioToChart</b>, <b>YRatioToChart</b>, <b>WidthRatioToChart</b> and <b>HeightRatioToChart</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> InnerY in Pixel = InnerYRatioToChart * chart.ChartObject.Width. Note: When InnerYRatioToChart is set, the IsInnerMode property will be automatically set to True.

### innerHeightRatioToChart {#innerHeightRatioToChart--}

Gets or sets the height of plot area in units of ratio of the chart area.

```javascript
innerHeightRatioToChart : number;
```


**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>XRatioToChart</b>, <b>YRatioToChart</b>, <b>WidthRatioToChart</b> and <b>HeightRatioToChart</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> InnerHeight in Pixel = InnerXRatioToChart * chart.ChartObject.Width. Note: When InnerHeightRatioToChart is set, the IsInnerMode property will be automatically set to True.

### innerWidthRatioToChart {#innerWidthRatioToChart--}

Gets or sets the width  of plot area in units of ratio of the chart area.

```javascript
innerWidthRatioToChart : number;
```


**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>XRatioToChart</b>, <b>YRatioToChart</b>, <b>WidthRatioToChart</b> and <b>HeightRatioToChart</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> InnerWidth in Pixel = InnerXRatioToChart * chart.ChartObject.Width. Note: When InnerWidthRatioToChart is set, the IsInnerMode property will be automatically set to True.

### isInnerMode {#isInnerMode--}

Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels.

```javascript
isInnerMode : boolean;
```


**Remarks**

Only for Xlsx file.

### backgroundMode {#backgroundMode--}

Gets and sets the display mode of the background

```javascript
backgroundMode : BackgroundMode;
```


### shadow {#shadow--}

True if the frame has a shadow.

```javascript
shadow : boolean;
```


### shapeProperties {#shapeProperties--}

Readonly. Gets the [ShapeProperties](../shapeproperties/) object.

```javascript
shapeProperties : ShapePropertyCollection;
```


### isDefaultPosBeSet {#isDefaultPosBeSet--}

Readonly. Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set.

```javascript
isDefaultPosBeSet : boolean;
```


### defaultX {#defaultX--}

Readonly. Represents x of default position in units of 1/4000 of the chart area.

```javascript
defaultX : number;
```


**Remarks**

NOTE: This member is now obsolete. Please use ChartFrame.DefaultXRatioToChart property, instead. DefaultX = (int)(DefaultXRatioToChart * 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### defaultY {#defaultY--}

Readonly. Represents y of default position in units of 1/4000 of the chart area.

```javascript
defaultY : number;
```


**Remarks**

NOTE: This member is now obsolete. Please use ChartFrame.DefaultYRatioToChart property, instead. DefaultY = (int)(DefaultYRatioToChart * 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### defaultWidth {#defaultWidth--}

Readonly. Represents width of default position in units of 1/4000 of the chart area.

```javascript
defaultWidth : number;
```


**Remarks**

NOTE: This member is now obsolete. Please use ChartFrame.DefaultWidthRatioToChart property, instead. DefaultWidth = (int)(DefaultWidthRatioToChart * 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### defaultHeight {#defaultHeight--}

Readonly. Represents height of default position in units of 1/4000 of the chart area.

```javascript
defaultHeight : number;
```


**Remarks**

NOTE: This member is now obsolete. Please use ChartFrame.DefaultHeightRatioToChart property, instead. DefaultHeight = (int)(DefaultHeightRatioToChart * 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### defaultXRatioToChart {#defaultXRatioToChart--}

Readonly. Represents x of default position in units of Fraction of the chart area.

```javascript
defaultXRatioToChart : number;
```


### defaultYRatioToChart {#defaultYRatioToChart--}

Readonly. Represents y of default position in units of Fraction of the chart area.

```javascript
defaultYRatioToChart : number;
```


### defaultWidthRatioToChart {#defaultWidthRatioToChart--}

Readonly. Represents width of default position in units of Fraction of the chart area.

```javascript
defaultWidthRatioToChart : number;
```


### defaultHeightRatioToChart {#defaultHeightRatioToChart--}

Readonly. Represents height of default position in units of Fraction of the chart area.

```javascript
defaultHeightRatioToChart : number;
```


### getInnerX() {#getInnerX--}

<b>@deprecated.</b> Please use the 'innerX' property instead. Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area.

```javascript
getInnerX() : number;
```


**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> Note: When InnerX is set, the IsInnerMode property will be automatically set to True.

### setInnerX(number) {#setInnerX-number-}

<b>@deprecated.</b> Please use the 'innerX' property instead. Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area.

```javascript
setInnerX(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> Note: When InnerX is set, the IsInnerMode property will be automatically set to True.

### getInnerY() {#getInnerY--}

<b>@deprecated.</b> Please use the 'innerY' property instead. Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area.

```javascript
getInnerY() : number;
```


**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> Note: When InnerY is set, the IsInnerMode property will be automatically set to True.

### setInnerY(number) {#setInnerY-number-}

<b>@deprecated.</b> Please use the 'innerY' property instead. Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area.

```javascript
setInnerY(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> Note: When InnerY is set, the IsInnerMode property will be automatically set to True.

### getInnerHeight() {#getInnerHeight--}

<b>@deprecated.</b> Please use the 'innerHeight' property instead. Gets or sets the height of plot area in units of 1/4000 of the chart area.

```javascript
getInnerHeight() : number;
```


**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> Note: When InnerHeight is set, the IsInnerMode property will be automatically set to True.

### setInnerHeight(number) {#setInnerHeight-number-}

<b>@deprecated.</b> Please use the 'innerHeight' property instead. Gets or sets the height of plot area in units of 1/4000 of the chart area.

```javascript
setInnerHeight(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> Note: When InnerHeight is set, the IsInnerMode property will be automatically set to True.

### getInnerWidth() {#getInnerWidth--}

<b>@deprecated.</b> Please use the 'innerWidth' property instead. Gets or sets the width  of plot area in units of 1/4000 of the chart area.

```javascript
getInnerWidth() : number;
```


**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> Note: When InnerWidth is set, the IsInnerMode property will be automatically set to True.

### setInnerWidth(number) {#setInnerWidth-number-}

<b>@deprecated.</b> Please use the 'innerWidth' property instead. Gets or sets the width  of plot area in units of 1/4000 of the chart area.

```javascript
setInnerWidth(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> Note: When InnerWidth is set, the IsInnerMode property will be automatically set to True.

### getInnerXRatioToChart() {#getInnerXRatioToChart--}

<b>@deprecated.</b> Please use the 'innerXRatioToChart' property instead. Gets or gets the x coordinate of the upper top corner of plot area in units of ratio of the chart area.

```javascript
getInnerXRatioToChart() : number;
```


**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>XRatioToChart</b>, <b>YRatioToChart</b>, <b>WidthRatioToChart</b> and <b>HeightRatioToChart</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> InnerX in Pixel = InnerXRatioToChart * chart.ChartObject.Width. Note: When InnerXRatioToChart is set, the IsInnerMode property will be automatically set to True.

### setInnerXRatioToChart(number) {#setInnerXRatioToChart-number-}

<b>@deprecated.</b> Please use the 'innerXRatioToChart' property instead. Gets or gets the x coordinate of the upper top corner of plot area in units of ratio of the chart area.

```javascript
setInnerXRatioToChart(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>XRatioToChart</b>, <b>YRatioToChart</b>, <b>WidthRatioToChart</b> and <b>HeightRatioToChart</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> InnerX in Pixel = InnerXRatioToChart * chart.ChartObject.Width. Note: When InnerXRatioToChart is set, the IsInnerMode property will be automatically set to True.

### getInnerYRatioToChart() {#getInnerYRatioToChart--}

<b>@deprecated.</b> Please use the 'innerYRatioToChart' property instead. Gets or gets the x coordinate of the upper top corner of plot area in units of ratio of the chart area.

```javascript
getInnerYRatioToChart() : number;
```


**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>XRatioToChart</b>, <b>YRatioToChart</b>, <b>WidthRatioToChart</b> and <b>HeightRatioToChart</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> InnerY in Pixel = InnerYRatioToChart * chart.ChartObject.Width. Note: When InnerYRatioToChart is set, the IsInnerMode property will be automatically set to True.

### setInnerYRatioToChart(number) {#setInnerYRatioToChart-number-}

<b>@deprecated.</b> Please use the 'innerYRatioToChart' property instead. Gets or gets the x coordinate of the upper top corner of plot area in units of ratio of the chart area.

```javascript
setInnerYRatioToChart(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>XRatioToChart</b>, <b>YRatioToChart</b>, <b>WidthRatioToChart</b> and <b>HeightRatioToChart</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> InnerY in Pixel = InnerYRatioToChart * chart.ChartObject.Width. Note: When InnerYRatioToChart is set, the IsInnerMode property will be automatically set to True.

### getInnerHeightRatioToChart() {#getInnerHeightRatioToChart--}

<b>@deprecated.</b> Please use the 'innerHeightRatioToChart' property instead. Gets or sets the height of plot area in units of ratio of the chart area.

```javascript
getInnerHeightRatioToChart() : number;
```


**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>XRatioToChart</b>, <b>YRatioToChart</b>, <b>WidthRatioToChart</b> and <b>HeightRatioToChart</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> InnerHeight in Pixel = InnerXRatioToChart * chart.ChartObject.Width. Note: When InnerHeightRatioToChart is set, the IsInnerMode property will be automatically set to True.

### setInnerHeightRatioToChart(number) {#setInnerHeightRatioToChart-number-}

<b>@deprecated.</b> Please use the 'innerHeightRatioToChart' property instead. Gets or sets the height of plot area in units of ratio of the chart area.

```javascript
setInnerHeightRatioToChart(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>XRatioToChart</b>, <b>YRatioToChart</b>, <b>WidthRatioToChart</b> and <b>HeightRatioToChart</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> InnerHeight in Pixel = InnerXRatioToChart * chart.ChartObject.Width. Note: When InnerHeightRatioToChart is set, the IsInnerMode property will be automatically set to True.

### getInnerWidthRatioToChart() {#getInnerWidthRatioToChart--}

<b>@deprecated.</b> Please use the 'innerWidthRatioToChart' property instead. Gets or sets the width  of plot area in units of ratio of the chart area.

```javascript
getInnerWidthRatioToChart() : number;
```


**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>XRatioToChart</b>, <b>YRatioToChart</b>, <b>WidthRatioToChart</b> and <b>HeightRatioToChart</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> InnerWidth in Pixel = InnerXRatioToChart * chart.ChartObject.Width. Note: When InnerWidthRatioToChart is set, the IsInnerMode property will be automatically set to True.

### setInnerWidthRatioToChart(number) {#setInnerWidthRatioToChart-number-}

<b>@deprecated.</b> Please use the 'innerWidthRatioToChart' property instead. Gets or sets the width  of plot area in units of ratio of the chart area.

```javascript
setInnerWidthRatioToChart(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>XRatioToChart</b>, <b>YRatioToChart</b>, <b>WidthRatioToChart</b> and <b>HeightRatioToChart</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> InnerWidth in Pixel = InnerXRatioToChart * chart.ChartObject.Width. Note: When InnerWidthRatioToChart is set, the IsInnerMode property will be automatically set to True.

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### isInnerMode() {#isInnerMode--}

<b>@deprecated.</b> Please use the 'isInnerMode' property instead. Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels.

```javascript
isInnerMode() : boolean;
```


**Remarks**

Only for Xlsx file.

### setIsInnerMode(boolean) {#setIsInnerMode-boolean-}

<b>@deprecated.</b> Please use the 'isInnerMode' property instead. Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels.

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

<b>@deprecated.</b> Please use the 'backgroundMode' property instead. Gets and sets the display mode of the background

```javascript
getBackgroundMode() : BackgroundMode;
```


**Returns**

[BackgroundMode](../backgroundmode/)

### setBackgroundMode(BackgroundMode) {#setBackgroundMode-backgroundmode-}

<b>@deprecated.</b> Please use the 'backgroundMode' property instead. Gets and sets the display mode of the background

```javascript
setBackgroundMode(value: BackgroundMode) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [BackgroundMode](../backgroundmode/) | The value to set. |

### getShadow() {#getShadow--}

<b>@deprecated.</b> Please use the 'shadow' property instead. True if the frame has a shadow.

```javascript
getShadow() : boolean;
```


### setShadow(boolean) {#setShadow-boolean-}

<b>@deprecated.</b> Please use the 'shadow' property instead. True if the frame has a shadow.

```javascript
setShadow(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShapeProperties() {#getShapeProperties--}

<b>@deprecated.</b> Please use the 'shapeProperties' property instead. Gets the [ShapeProperties](../shapeproperties/) object.

```javascript
getShapeProperties() : ShapePropertyCollection;
```


**Returns**

[ShapePropertyCollection](../shapepropertycollection/)

### isDefaultPosBeSet() {#isDefaultPosBeSet--}

<b>@deprecated.</b> Please use the 'isDefaultPosBeSet' property instead. Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set.

```javascript
isDefaultPosBeSet() : boolean;
```


### getDefaultX() {#getDefaultX--}

<b>@deprecated.</b> Please use the 'defaultX' property instead. Represents x of default position in units of 1/4000 of the chart area.

```javascript
getDefaultX() : number;
```


**Remarks**

NOTE: This member is now obsolete. Please use ChartFrame.DefaultXRatioToChart property, instead. DefaultX = (int)(DefaultXRatioToChart * 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### getDefaultY() {#getDefaultY--}

<b>@deprecated.</b> Please use the 'defaultY' property instead. Represents y of default position in units of 1/4000 of the chart area.

```javascript
getDefaultY() : number;
```


**Remarks**

NOTE: This member is now obsolete. Please use ChartFrame.DefaultYRatioToChart property, instead. DefaultY = (int)(DefaultYRatioToChart * 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### getDefaultWidth() {#getDefaultWidth--}

<b>@deprecated.</b> Please use the 'defaultWidth' property instead. Represents width of default position in units of 1/4000 of the chart area.

```javascript
getDefaultWidth() : number;
```


**Remarks**

NOTE: This member is now obsolete. Please use ChartFrame.DefaultWidthRatioToChart property, instead. DefaultWidth = (int)(DefaultWidthRatioToChart * 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### getDefaultHeight() {#getDefaultHeight--}

<b>@deprecated.</b> Please use the 'defaultHeight' property instead. Represents height of default position in units of 1/4000 of the chart area.

```javascript
getDefaultHeight() : number;
```


**Remarks**

NOTE: This member is now obsolete. Please use ChartFrame.DefaultHeightRatioToChart property, instead. DefaultHeight = (int)(DefaultHeightRatioToChart * 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### getDefaultXRatioToChart() {#getDefaultXRatioToChart--}

<b>@deprecated.</b> Please use the 'defaultXRatioToChart' property instead. Represents x of default position in units of Fraction of the chart area.

```javascript
getDefaultXRatioToChart() : number;
```


### getDefaultYRatioToChart() {#getDefaultYRatioToChart--}

<b>@deprecated.</b> Please use the 'defaultYRatioToChart' property instead. Represents y of default position in units of Fraction of the chart area.

```javascript
getDefaultYRatioToChart() : number;
```


### getDefaultWidthRatioToChart() {#getDefaultWidthRatioToChart--}

<b>@deprecated.</b> Please use the 'defaultWidthRatioToChart' property instead. Represents width of default position in units of Fraction of the chart area.

```javascript
getDefaultWidthRatioToChart() : number;
```


### getDefaultHeightRatioToChart() {#getDefaultHeightRatioToChart--}

<b>@deprecated.</b> Please use the 'defaultHeightRatioToChart' property instead. Represents height of default position in units of Fraction of the chart area.

```javascript
getDefaultHeightRatioToChart() : number;
```


### getX() {#getX--}

Gets or gets the x coordinate of the upper left corner of plot-area bounding box in units of 1/4000 of the chart area.

```javascript
getX() : number;
```


**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> Note: When X is set, the IsInnerMode property will be automatically set to false.

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

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> Note: When X is set, the IsInnerMode property will be automatically set to false.

### getY() {#getY--}

Gets or gets the y coordinate of the upper top corner  of plot-area bounding box in units of 1/4000 of the chart area.

```javascript
getY() : number;
```


**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> Note: When Y is set, the IsInnerMode property will be automatically set to false.

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

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> Note: When Y is set, the IsInnerMode property will be automatically set to false.

### getHeight() {#getHeight--}

Gets or sets the height of plot-area bounding box in units of 1/4000 of the chart area.

```javascript
getHeight() : number;
```


**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> Note: When Height is set, the IsInnerMode property will be automatically set to false.

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

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> Note: When Height is set, the IsInnerMode property will be automatically set to false.

### getWidth() {#getWidth--}

Gets or sets the width of plot-area bounding box in units of 1/4000 of the chart area.

```javascript
getWidth() : number;
```


**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> Note: When Width is set, the IsInnerMode property will be automatically set to false.

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

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>X</b>, <b>Y</b>, <b>Width</b> and <b>Height</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> Note: When Width is set, the IsInnerMode property will be automatically set to false.

### getXRatioToChart() {#getXRatioToChart--}

Gets or gets the x coordinate of the upper left corner of plot-area bounding box in units of ratio of the chart area.

```javascript
getXRatioToChart() : number;
```


**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>XRatioToChart</b>, <b>YRatioToChart</b>, <b>WidthRatioToChart</b> and <b>HeightRatioToChart</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> XPixel = XRatioToChart * chart.ChartObject.Width. Note: When XRatioToChart is set, the IsInnerMode property will be automatically set to false.

### setXRatioToChart(number) {#setXRatioToChart-number-}

Gets or gets the x coordinate of the upper left corner of plot-area bounding box in units of ratio of the chart area.

```javascript
setXRatioToChart(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>XRatioToChart</b>, <b>YRatioToChart</b>, <b>WidthRatioToChart</b> and <b>HeightRatioToChart</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> XPixel = XRatioToChart * chart.ChartObject.Width. Note: When XRatioToChart is set, the IsInnerMode property will be automatically set to false.

### getYRatioToChart() {#getYRatioToChart--}

Gets or gets the y coordinate of the upper top corner  of plot-area bounding box in units of ratio of the chart area.

```javascript
getYRatioToChart() : number;
```


**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>XRatioToChart</b>, <b>YRatioToChart</b>, <b>WidthRatioToChart</b> and <b>HeightRatioToChart</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> YPixel = YRatioToChart * chart.ChartObject.Width. Note: When YRatioToChart is set, the IsInnerMode property will be automatically set to false.

### setYRatioToChart(number) {#setYRatioToChart-number-}

Gets or gets the y coordinate of the upper top corner  of plot-area bounding box in units of ratio of the chart area.

```javascript
setYRatioToChart(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>XRatioToChart</b>, <b>YRatioToChart</b>, <b>WidthRatioToChart</b> and <b>HeightRatioToChart</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> YPixel = YRatioToChart * chart.ChartObject.Width. Note: When YRatioToChart is set, the IsInnerMode property will be automatically set to false.

### getHeightRatioToChart() {#getHeightRatioToChart--}

Gets or sets the height of plot-area bounding box in units of ratio of the chart area.

```javascript
getHeightRatioToChart() : number;
```


**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>XRatioToChart</b>, <b>YRatioToChart</b>, <b>WidthRatioToChart</b> and <b>HeightRatioToChart</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> HeightPixel = HeightRatioToChart * chart.ChartObject.Width. Note: When HeightRatioToChart is set, the IsInnerMode property will be automatically set to false.

### setHeightRatioToChart(number) {#setHeightRatioToChart-number-}

Gets or sets the height of plot-area bounding box in units of ratio of the chart area.

```javascript
setHeightRatioToChart(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>XRatioToChart</b>, <b>YRatioToChart</b>, <b>WidthRatioToChart</b> and <b>HeightRatioToChart</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> HeightPixel = HeightRatioToChart * chart.ChartObject.Width. Note: When HeightRatioToChart is set, the IsInnerMode property will be automatically set to false.

### getWidthRatioToChart() {#getWidthRatioToChart--}

Gets or sets the width of plot-area bounding box in units of ratio of the chart area.

```javascript
getWidthRatioToChart() : number;
```


**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>XRatioToChart</b>, <b>YRatioToChart</b>, <b>WidthRatioToChart</b> and <b>HeightRatioToChart</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> WidthPixel = WidthRatioToChart * chart.ChartObject.Width. Note: When WidthRatioToChart is set, the IsInnerMode property will be automatically set to false.

### setWidthRatioToChart(number) {#setWidthRatioToChart-number-}

Gets or sets the width of plot-area bounding box in units of ratio of the chart area.

```javascript
setWidthRatioToChart(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. </p> <p>The <b>XRatioToChart</b>, <b>YRatioToChart</b>, <b>WidthRatioToChart</b> and <b>HeightRatioToChart</b> of <b>PlotArea</b> represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call <b>InnerXRatioToChart</b>, <b>InnerYRatioToChart</b>, <b>InnerWidthRatioToChart</b> and <b>InnerHeightRatioToChart</b> properties.</p> <p>For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().</p> WidthPixel = WidthRatioToChart * chart.ChartObject.Width. Note: When WidthRatioToChart is set, the IsInnerMode property will be automatically set to false.

### isAutomaticSize() {#isAutomaticSize--}

Indicates whether the plot area is automatic sized.

```javascript
isAutomaticSize() : boolean;
```


**Remarks**

NOTE: When IsAutomaticSize is set to True, the values you manually set for Width and Height will be disabled.

### setIsAutomaticSize(boolean) {#setIsAutomaticSize-boolean-}

Indicates whether the plot area is automatic sized.

```javascript
setIsAutomaticSize(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

NOTE: When IsAutomaticSize is set to True, the values you manually set for Width and Height will be disabled.

### setPositionAuto() {#setPositionAuto--}

Set position of the plot area to automatic

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


