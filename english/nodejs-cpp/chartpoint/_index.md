---
title: ChartPoint
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a single point in a series in a chart.
type: docs
url: /nodejs-cpp/chartpoint/
---

## ChartPoint class

Represents a single point in a series in a chart.

```javascript
class ChartPoint;
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
var chartIndex = worksheet.getCharts().add(ChartType.PieExploded, 5, 0, 25, 10);
//Accessing the instance of the newly added chart
var chart = worksheet.getCharts().get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.getNSeries().add("A1:B3", true);
//Show Data Labels 
chart.getNSeries().get(0).getDataLabels().setShowValue(true);
for (var i = 0; i < chart.getNSeries().get(0).getPoints().getCount(); i++) {
    //Get Data Point
    var point = chart.getNSeries().get(0).getPoints().get(i);
    //Set Pir Explosion
    point.setExplosion(15);
    //Set Border Color
    point.getBorder().setColor(Color.Red);
}

//Saving the Excel file
workbook.save("output/ChartsChartPoint.xls");
```
## Methods

| Method | Description |
| --- | --- |
| [getExplosion()](#getExplosion--)| The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [setExplosion(number)](#setExplosion-number-)| The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [getShadow()](#getShadow--)| True if the chartpoint has a shadow. |
| [setShadow(boolean)](#setShadow-boolean-)| True if the chartpoint has a shadow. |
| [getBorder()](#getBorder--)| Gets the <see cref="Line"> border</see>. |
| [getArea()](#getArea--)| Gets the <see cref="Area"> area</see>. |
| [getMarker()](#getMarker--)| Gets the <see cref="Marker"> marker</see>. |
| [getDataLabels()](#getDataLabels--)| Returns a [DataLabels](../datalabels/) object that represents the data label associated with this chart point. |
| [get_YValue()](#get_YValue--)| Gets or sets the Y value of the chart point. |
| [setYValue(Object)](#setYValue-object-)| Gets or sets the Y value of the chart point. |
| [getYValueType()](#getYValueType--)| Gets Y value type of the chart point. |
| [getXValue()](#getXValue--)| Gets or sets the X value of the chart point. |
| [setXValue(Object)](#setXValue-object-)| Gets or sets the X value of the chart point. |
| [getXValueType()](#getXValueType--)| Gets X value type of the chart point. |
| [getShapeProperties()](#getShapeProperties--)| Gets the [ShapePropertyCollection](../shapepropertycollection/) object that holds the visual shape properties of the ChartPoint. |
| [isInSecondaryPlot()](#isInSecondaryPlot--)| Gets or sets a value indicates whether this data points is in the second pie or bar on a pie of pie or bar of pie chart |
| [setIsInSecondaryPlot(boolean)](#setIsInSecondaryPlot-boolean-)| Gets or sets a value indicates whether this data points is in the second pie or bar on a pie of pie or bar of pie chart |
| [getShapeX()](#getShapeX--)| Gets the x coordinate of the upper left corner in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [getShapeY()](#getShapeY--)| Gets the y coordinate of the upper left corner in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [getShapeWidth()](#getShapeWidth--)| Gets the width in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [getShapeHeight()](#getShapeHeight--)| Gets the height in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [getShapeXPx()](#getShapeXPx--)| Gets the x coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method. |
| [getShapeYPx()](#getShapeYPx--)| Gets the y coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method. |
| [getShapeWidthPx()](#getShapeWidthPx--)| Gets the width in units of pixels after calls Chart.Calculate() method. |
| [getShapeHeightPx()](#getShapeHeightPx--)| Gets the height in units of pixels after calls Chart.Calculate() method. |
| [getBorderWidthPx()](#getBorderWidthPx--)| Gets the width of border in units of pixels after calls Chart.Calculate() method. |
| [getRadiusPx()](#getRadiusPx--)| Gets the radius of bubble, pie or doughnut in units of pixels after calls Chart.Calculate() method. |
| [getDoughnutInnerRadius()](#getDoughnutInnerRadius--)| Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method. Applies to Doughnut chart. |
| [getInnerRadiusPx()](#getInnerRadiusPx--)| Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method. Applies to Doughnut chart. |
| [getStartAngle()](#getStartAngle--)| Gets the starting angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method. Applies to Pie chart. |
| [getEndAngle()](#getEndAngle--)| Gets the ending angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method. Applies to Pie chart. |
| [getArcStartPointXPx()](#getArcStartPointXPx--)| Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut  chart. |
| [getArcStartPointYPx()](#getArcStartPointYPx--)| Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut  chart. |
| [getArcEndPointXPx()](#getArcEndPointXPx--)| Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut  chart. |
| [getArcEndPointYPx()](#getArcEndPointYPx--)| Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart. |
| [getInnerArcStartPointXPx()](#getInnerArcStartPointXPx--)| Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart. |
| [getInnerArcStartPointYPx()](#getInnerArcStartPointYPx--)| Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart. |
| [getInnerArcEndPointXPx()](#getInnerArcEndPointXPx--)| Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart. |
| [getInnerArcEndPointYPx()](#getInnerArcEndPointYPx--)| Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart. |
| [getTopPointCount()](#getTopPointCount--)| Gets the number of top points after calls Chart.Calculate() method. |
| [getTopPointXPx(number)](#getTopPointXPx-number-)| Gets x-coordinate of the top point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid and Area3D |
| [getTopPointYPx(number)](#getTopPointYPx-number-)| Gets y-coordinate of the top point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid and Area3D |
| [getBottomPointCount()](#getBottomPointCount--)| Gets the number of bottom points  after calls Chart.Calculate() method. |
| [getBottomPointXPx(number)](#getBottomPointXPx-number-)| Gets x-coordinate of the bottom point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid |
| [getBottomPointYPx(number)](#getBottomPointYPx-number-)| Gets y-coordinate of the bottom point of shape  after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid |
| [getOnCategoryAxisPointCount()](#getOnCategoryAxisPointCount--)| Gets the number of the points on category axis after calls Chart.Calculate() method. Only applies to area chart. |
| [getOnCategoryAxisPointXPx(number)](#getOnCategoryAxisPointXPx-number-)| Gets x-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart. |
| [getOnCategoryAxisPointYPx(number)](#getOnCategoryAxisPointYPx-number-)| Gets y-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getExplosion() {#getExplosion--}

The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter.

```javascript
getExplosion() : number;
```


### setExplosion(number) {#setExplosion-number-}

The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter.

```javascript
setExplosion(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getShadow() {#getShadow--}

True if the chartpoint has a shadow.

```javascript
getShadow() : boolean;
```


### setShadow(boolean) {#setShadow-boolean-}

True if the chartpoint has a shadow.

```javascript
setShadow(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getBorder() {#getBorder--}

Gets the <see cref="Line"> border</see>.

```javascript
getBorder() : Line;
```


**Returns**

[Line](../line/)

### getArea() {#getArea--}

Gets the <see cref="Area"> area</see>.

```javascript
getArea() : Area;
```


**Returns**

[Area](../area/)

### getMarker() {#getMarker--}

Gets the <see cref="Marker"> marker</see>.

```javascript
getMarker() : Marker;
```


**Returns**

[Marker](../marker/)

### getDataLabels() {#getDataLabels--}

Returns a [DataLabels](../datalabels/) object that represents the data label associated with this chart point.

```javascript
getDataLabels() : DataLabels;
```


**Returns**

[DataLabels](../datalabels/)

### get_YValue() {#get_YValue--}

Gets or sets the Y value of the chart point.

```javascript
get_YValue() : Object;
```


### setYValue(Object) {#setYValue-object-}

Gets or sets the Y value of the chart point.

```javascript
setYValue(value: Object) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | The value to set. |

### getYValueType() {#getYValueType--}

Gets Y value type of the chart point.

```javascript
getYValueType() : CellValueType;
```


**Returns**

[CellValueType](../cellvaluetype/)

### getXValue() {#getXValue--}

Gets or sets the X value of the chart point.

```javascript
getXValue() : Object;
```


### setXValue(Object) {#setXValue-object-}

Gets or sets the X value of the chart point.

```javascript
setXValue(value: Object) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | The value to set. |

### getXValueType() {#getXValueType--}

Gets X value type of the chart point.

```javascript
getXValueType() : CellValueType;
```


**Returns**

[CellValueType](../cellvaluetype/)

### getShapeProperties() {#getShapeProperties--}

Gets the [ShapePropertyCollection](../shapepropertycollection/) object that holds the visual shape properties of the ChartPoint.

```javascript
getShapeProperties() : ShapePropertyCollection;
```


**Returns**

[ShapePropertyCollection](../shapepropertycollection/)

### isInSecondaryPlot() {#isInSecondaryPlot--}

Gets or sets a value indicates whether this data points is in the second pie or bar on a pie of pie or bar of pie chart

```javascript
isInSecondaryPlot() : boolean;
```


### setIsInSecondaryPlot(boolean) {#setIsInSecondaryPlot-boolean-}

Gets or sets a value indicates whether this data points is in the second pie or bar on a pie of pie or bar of pie chart

```javascript
setIsInSecondaryPlot(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShapeX() {#getShapeX--}

Gets the x coordinate of the upper left corner in units of 1/4000 of chart's width after calls Chart.Calculate() method.

```javascript
getShapeX() : number;
```


### getShapeY() {#getShapeY--}

Gets the y coordinate of the upper left corner in units of 1/4000 of chart's height after calls Chart.Calculate() method.

```javascript
getShapeY() : number;
```


### getShapeWidth() {#getShapeWidth--}

Gets the width in units of 1/4000 of chart's width after calls Chart.Calculate() method.

```javascript
getShapeWidth() : number;
```


### getShapeHeight() {#getShapeHeight--}

Gets the height in units of 1/4000 of chart's height after calls Chart.Calculate() method.

```javascript
getShapeHeight() : number;
```


### getShapeXPx() {#getShapeXPx--}

Gets the x coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method.

```javascript
getShapeXPx() : number;
```


### getShapeYPx() {#getShapeYPx--}

Gets the y coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method.

```javascript
getShapeYPx() : number;
```


### getShapeWidthPx() {#getShapeWidthPx--}

Gets the width in units of pixels after calls Chart.Calculate() method.

```javascript
getShapeWidthPx() : number;
```


### getShapeHeightPx() {#getShapeHeightPx--}

Gets the height in units of pixels after calls Chart.Calculate() method.

```javascript
getShapeHeightPx() : number;
```


### getBorderWidthPx() {#getBorderWidthPx--}

Gets the width of border in units of pixels after calls Chart.Calculate() method.

```javascript
getBorderWidthPx() : number;
```


### getRadiusPx() {#getRadiusPx--}

Gets the radius of bubble, pie or doughnut in units of pixels after calls Chart.Calculate() method.

```javascript
getRadiusPx() : number;
```


### getDoughnutInnerRadius() {#getDoughnutInnerRadius--}

Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method. Applies to Doughnut chart.

```javascript
getDoughnutInnerRadius() : number;
```


### getInnerRadiusPx() {#getInnerRadiusPx--}

Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method. Applies to Doughnut chart.

```javascript
getInnerRadiusPx() : number;
```


**Remarks**

NOTE: This property is now obsolete. Instead, please use ChartPoint.DoughnutInnerRadius property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### getStartAngle() {#getStartAngle--}

Gets the starting angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method. Applies to Pie chart.

```javascript
getStartAngle() : number;
```


### getEndAngle() {#getEndAngle--}

Gets the ending angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method. Applies to Pie chart.

```javascript
getEndAngle() : number;
```


### getArcStartPointXPx() {#getArcStartPointXPx--}

Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut  chart.

```javascript
getArcStartPointXPx() : number;
```


### getArcStartPointYPx() {#getArcStartPointYPx--}

Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut  chart.

```javascript
getArcStartPointYPx() : number;
```


### getArcEndPointXPx() {#getArcEndPointXPx--}

Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut  chart.

```javascript
getArcEndPointXPx() : number;
```


### getArcEndPointYPx() {#getArcEndPointYPx--}

Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart.

```javascript
getArcEndPointYPx() : number;
```


### getInnerArcStartPointXPx() {#getInnerArcStartPointXPx--}

Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart.

```javascript
getInnerArcStartPointXPx() : number;
```


### getInnerArcStartPointYPx() {#getInnerArcStartPointYPx--}

Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart.

```javascript
getInnerArcStartPointYPx() : number;
```


### getInnerArcEndPointXPx() {#getInnerArcEndPointXPx--}

Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart.

```javascript
getInnerArcEndPointXPx() : number;
```


### getInnerArcEndPointYPx() {#getInnerArcEndPointYPx--}

Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart.

```javascript
getInnerArcEndPointYPx() : number;
```


### getTopPointCount() {#getTopPointCount--}

Gets the number of top points after calls Chart.Calculate() method.

```javascript
getTopPointCount() : number;
```


### getTopPointXPx(number) {#getTopPointXPx-number-}

Gets x-coordinate of the top point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid and Area3D

```javascript
getTopPointXPx(index: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |

### getTopPointYPx(number) {#getTopPointYPx-number-}

Gets y-coordinate of the top point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid and Area3D

```javascript
getTopPointYPx(index: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |

### getBottomPointCount() {#getBottomPointCount--}

Gets the number of bottom points  after calls Chart.Calculate() method.

```javascript
getBottomPointCount() : number;
```


### getBottomPointXPx(number) {#getBottomPointXPx-number-}

Gets x-coordinate of the bottom point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid

```javascript
getBottomPointXPx(index: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |

### getBottomPointYPx(number) {#getBottomPointYPx-number-}

Gets y-coordinate of the bottom point of shape  after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid

```javascript
getBottomPointYPx(index: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |

### getOnCategoryAxisPointCount() {#getOnCategoryAxisPointCount--}

Gets the number of the points on category axis after calls Chart.Calculate() method. Only applies to area chart.

```javascript
getOnCategoryAxisPointCount() : number;
```


**Remarks**

Area 2D chart return 1 Area 3D chart return 2.

### getOnCategoryAxisPointXPx(number) {#getOnCategoryAxisPointXPx-number-}

Gets x-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart.

```javascript
getOnCategoryAxisPointXPx(index: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |

**Remarks**

Area 2D chart: index is 0. Area 3D chart: index is 0 or 1.

### getOnCategoryAxisPointYPx(number) {#getOnCategoryAxisPointYPx-number-}

Gets y-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart.

```javascript
getOnCategoryAxisPointYPx(index: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |

**Remarks**

Area 2D chart: index is 0. Area 3D chart: index is 0 or 1.

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



