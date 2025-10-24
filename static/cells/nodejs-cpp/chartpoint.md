##ChartPoint
Represents a single point in a series in a chart.
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
var worksheet = workbook.worksheets.get(0);
//Adding a sample value to "A1" cell
worksheet.cells.get("A1").putValue(50);
//Adding a sample value to "A2" cell
worksheet.cells.get("A2").putValue(100);
//Adding a sample value to "A3" cell
worksheet.cells.get("A3").putValue(150);
//Adding a sample value to "B1" cell
worksheet.cells.get("B1").putValue(60);
//Adding a sample value to "B2" cell
worksheet.cells.get("B2").putValue(32);
//Adding a sample value to "B3" cell
worksheet.cells.get("B3").putValue(50);
//Adding a chart to the worksheet
var chartIndex = worksheet.charts.add(ChartType.PieExploded, 5, 0, 25, 10);
//Accessing the instance of the newly added chart
var chart = worksheet.charts.get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.nSeries.add("A1:B3", true);
//Show Data Labels
chart.nSeries.get(0).dataLabels.showValue = true;
for (var i = 0; i < chart.nSeries.get(0).points.count; i++) {
//Get Data Point
var point = chart.nSeries.get(0).points.get(i);
//Set Pir Explosion
point.explosion = 15;
//Set Border Color
point.border.color = Color.Red;
}
//Saving the Excel file
workbook.save("output/ChartsChartPoint.xls");
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [explosion](#explosion--)| number | The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [shadow](#shadow--)| boolean | True if the chartpoint has a shadow. |
| [border](#border--)| Line | Readonly. Gets the <see cref="Line"> border</see>. |
| [area](#area--)| Area | Readonly. Gets the <see cref="Area"> area</see>. |
| [marker](#marker--)| Marker | Readonly. Gets the <see cref="Marker"> marker</see>. |
| [dataLabels](#dataLabels--)| DataLabels | Readonly. Returns a [DataLabels](../datalabels/) object that represents the data label associated with this chart point. |
| [yValue](#yValue--)| Object | Gets or sets the Y value of the chart point. |
| [yValueType](#yValueType--)| CellValueType | Readonly. Gets Y value type of the chart point. |
| [xValue](#xValue--)| Object | Gets or sets the X value of the chart point. |
| [xValueType](#xValueType--)| CellValueType | Readonly. Gets X value type of the chart point. |
| [shapeProperties](#shapeProperties--)| ShapePropertyCollection | Readonly. Gets the [ShapePropertyCollection](../shapepropertycollection/) object that holds the visual shape properties of the ChartPoint. |
| [isInSecondaryPlot](#isInSecondaryPlot--)| boolean | Gets or sets a value indicates whether this data points is in the second pie or bar on a pie of pie or bar of pie chart |
| [shapeX](#shapeX--)| number | Readonly. Gets the x coordinate of the upper left corner in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [shapeY](#shapeY--)| number | Readonly. Gets the y coordinate of the upper left corner in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [shapeWidth](#shapeWidth--)| number | Readonly. Gets the width in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [shapeHeight](#shapeHeight--)| number | Readonly. Gets the height in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [shapeXPx](#shapeXPx--)| number | Readonly. Gets the x coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method. |
| [shapeYPx](#shapeYPx--)| number | Readonly. Gets the y coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method. |
| [shapeWidthPx](#shapeWidthPx--)| number | Readonly. Gets the width in units of pixels after calls Chart.Calculate() method. |
| [shapeHeightPx](#shapeHeightPx--)| number | Readonly. Gets the height in units of pixels after calls Chart.Calculate() method. |
| [borderWidthPx](#borderWidthPx--)| number | Readonly. Gets the width of border in units of pixels after calls Chart.Calculate() method. |
| [radiusPx](#radiusPx--)| number | Readonly. Gets the radius of bubble, pie or doughnut in units of pixels after calls Chart.Calculate() method. |
| [doughnutInnerRadius](#doughnutInnerRadius--)| number | Readonly. Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method. Applies to Doughnut chart. |
| [innerRadiusPx](#innerRadiusPx--)| number | Readonly. Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method. Applies to Doughnut chart. |
| [startAngle](#startAngle--)| number | Readonly. Gets the starting angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method. Applies to Pie chart. |
| [endAngle](#endAngle--)| number | Readonly. Gets the ending angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method. Applies to Pie chart. |
| [arcStartPointXPx](#arcStartPointXPx--)| number | Readonly. Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut  chart. |
| [arcStartPointYPx](#arcStartPointYPx--)| number | Readonly. Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut  chart. |
| [arcEndPointXPx](#arcEndPointXPx--)| number | Readonly. Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut  chart. |
| [arcEndPointYPx](#arcEndPointYPx--)| number | Readonly. Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart. |
| [innerArcStartPointXPx](#innerArcStartPointXPx--)| number | Readonly. Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart. |
| [innerArcStartPointYPx](#innerArcStartPointYPx--)| number | Readonly. Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart. |
| [innerArcEndPointXPx](#innerArcEndPointXPx--)| number | Readonly. Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart. |
| [innerArcEndPointYPx](#innerArcEndPointYPx--)| number | Readonly. Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart. |
## Methods
| Method | Description |
| --- | --- |
| [getExplosion()](#getExplosion--)| <b>@deprecated.</b> Please use the 'explosion' property instead. The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [setExplosion(number)](#setExplosion-number-)| <b>@deprecated.</b> Please use the 'explosion' property instead. The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [getShadow()](#getShadow--)| <b>@deprecated.</b> Please use the 'shadow' property instead. True if the chartpoint has a shadow. |
| [setShadow(boolean)](#setShadow-boolean-)| <b>@deprecated.</b> Please use the 'shadow' property instead. True if the chartpoint has a shadow. |
| [getBorder()](#getBorder--)| <b>@deprecated.</b> Please use the 'border' property instead. Gets the <see cref="Line"> border</see>. |
| [getArea()](#getArea--)| <b>@deprecated.</b> Please use the 'area' property instead. Gets the <see cref="Area"> area</see>. |
| [getMarker()](#getMarker--)| <b>@deprecated.</b> Please use the 'marker' property instead. Gets the <see cref="Marker"> marker</see>. |
| [getDataLabels()](#getDataLabels--)| <b>@deprecated.</b> Please use the 'dataLabels' property instead. Returns a [DataLabels](../datalabels/) object that represents the data label associated with this chart point. |
| [get_YValue()](#get_YValue--)| <b>@deprecated.</b> Please use the 'yValue' property instead. Gets or sets the Y value of the chart point. |
| [setYValue(Object)](#setYValue-object-)| <b>@deprecated.</b> Please use the 'yValue' property instead. Gets or sets the Y value of the chart point. |
| [getYValueType()](#getYValueType--)| <b>@deprecated.</b> Please use the 'yValueType' property instead. Gets Y value type of the chart point. |
| [getXValue()](#getXValue--)| <b>@deprecated.</b> Please use the 'xValue' property instead. Gets or sets the X value of the chart point. |
| [setXValue(Object)](#setXValue-object-)| <b>@deprecated.</b> Please use the 'xValue' property instead. Gets or sets the X value of the chart point. |
| [getXValueType()](#getXValueType--)| <b>@deprecated.</b> Please use the 'xValueType' property instead. Gets X value type of the chart point. |
| [getShapeProperties()](#getShapeProperties--)| <b>@deprecated.</b> Please use the 'shapeProperties' property instead. Gets the [ShapePropertyCollection](../shapepropertycollection/) object that holds the visual shape properties of the ChartPoint. |
| [isInSecondaryPlot()](#isInSecondaryPlot--)| <b>@deprecated.</b> Please use the 'isInSecondaryPlot' property instead. Gets or sets a value indicates whether this data points is in the second pie or bar on a pie of pie or bar of pie chart |
| [setIsInSecondaryPlot(boolean)](#setIsInSecondaryPlot-boolean-)| <b>@deprecated.</b> Please use the 'isInSecondaryPlot' property instead. Gets or sets a value indicates whether this data points is in the second pie or bar on a pie of pie or bar of pie chart |
| [getShapeX()](#getShapeX--)| <b>@deprecated.</b> Please use the 'shapeX' property instead. Gets the x coordinate of the upper left corner in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [getShapeY()](#getShapeY--)| <b>@deprecated.</b> Please use the 'shapeY' property instead. Gets the y coordinate of the upper left corner in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [getShapeWidth()](#getShapeWidth--)| <b>@deprecated.</b> Please use the 'shapeWidth' property instead. Gets the width in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [getShapeHeight()](#getShapeHeight--)| <b>@deprecated.</b> Please use the 'shapeHeight' property instead. Gets the height in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [getShapeXPx()](#getShapeXPx--)| <b>@deprecated.</b> Please use the 'shapeXPx' property instead. Gets the x coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method. |
| [getShapeYPx()](#getShapeYPx--)| <b>@deprecated.</b> Please use the 'shapeYPx' property instead. Gets the y coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method. |
| [getShapeWidthPx()](#getShapeWidthPx--)| <b>@deprecated.</b> Please use the 'shapeWidthPx' property instead. Gets the width in units of pixels after calls Chart.Calculate() method. |
| [getShapeHeightPx()](#getShapeHeightPx--)| <b>@deprecated.</b> Please use the 'shapeHeightPx' property instead. Gets the height in units of pixels after calls Chart.Calculate() method. |
| [getBorderWidthPx()](#getBorderWidthPx--)| <b>@deprecated.</b> Please use the 'borderWidthPx' property instead. Gets the width of border in units of pixels after calls Chart.Calculate() method. |
| [getRadiusPx()](#getRadiusPx--)| <b>@deprecated.</b> Please use the 'radiusPx' property instead. Gets the radius of bubble, pie or doughnut in units of pixels after calls Chart.Calculate() method. |
| [getDoughnutInnerRadius()](#getDoughnutInnerRadius--)| <b>@deprecated.</b> Please use the 'doughnutInnerRadius' property instead. Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method. Applies to Doughnut chart. |
| [getInnerRadiusPx()](#getInnerRadiusPx--)| <b>@deprecated.</b> Please use the 'innerRadiusPx' property instead. Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method. Applies to Doughnut chart. |
| [getStartAngle()](#getStartAngle--)| <b>@deprecated.</b> Please use the 'startAngle' property instead. Gets the starting angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method. Applies to Pie chart. |
| [getEndAngle()](#getEndAngle--)| <b>@deprecated.</b> Please use the 'endAngle' property instead. Gets the ending angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method. Applies to Pie chart. |
| [getArcStartPointXPx()](#getArcStartPointXPx--)| <b>@deprecated.</b> Please use the 'arcStartPointXPx' property instead. Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut  chart. |
| [getArcStartPointYPx()](#getArcStartPointYPx--)| <b>@deprecated.</b> Please use the 'arcStartPointYPx' property instead. Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut  chart. |
| [getArcEndPointXPx()](#getArcEndPointXPx--)| <b>@deprecated.</b> Please use the 'arcEndPointXPx' property instead. Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut  chart. |
| [getArcEndPointYPx()](#getArcEndPointYPx--)| <b>@deprecated.</b> Please use the 'arcEndPointYPx' property instead. Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart. |
| [getInnerArcStartPointXPx()](#getInnerArcStartPointXPx--)| <b>@deprecated.</b> Please use the 'innerArcStartPointXPx' property instead. Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart. |
| [getInnerArcStartPointYPx()](#getInnerArcStartPointYPx--)| <b>@deprecated.</b> Please use the 'innerArcStartPointYPx' property instead. Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart. |
| [getInnerArcEndPointXPx()](#getInnerArcEndPointXPx--)| <b>@deprecated.</b> Please use the 'innerArcEndPointXPx' property instead. Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart. |
| [getInnerArcEndPointYPx()](#getInnerArcEndPointYPx--)| <b>@deprecated.</b> Please use the 'innerArcEndPointYPx' property instead. Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart. |
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
### explosion {#explosion--}
The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter.
```javascript
explosion : number;
```
### shadow {#shadow--}
True if the chartpoint has a shadow.
```javascript
shadow : boolean;
```
### border {#border--}
Readonly. Gets the <see cref="Line"> border</see>.
```javascript
border : Line;
```
### area {#area--}
Readonly. Gets the <see cref="Area"> area</see>.
```javascript
area : Area;
```
### marker {#marker--}
Readonly. Gets the <see cref="Marker"> marker</see>.
```javascript
marker : Marker;
```
### dataLabels {#dataLabels--}
Readonly. Returns a [DataLabels](../datalabels/) object that represents the data label associated with this chart point.
```javascript
dataLabels : DataLabels;
```
### yValue {#yValue--}
Gets or sets the Y value of the chart point.
```javascript
yValue : Object;
```
### yValueType {#yValueType--}
Readonly. Gets Y value type of the chart point.
```javascript
yValueType : CellValueType;
```
### xValue {#xValue--}
Gets or sets the X value of the chart point.
```javascript
xValue : Object;
```
### xValueType {#xValueType--}
Readonly. Gets X value type of the chart point.
```javascript
xValueType : CellValueType;
```
### shapeProperties {#shapeProperties--}
Readonly. Gets the [ShapePropertyCollection](../shapepropertycollection/) object that holds the visual shape properties of the ChartPoint.
```javascript
shapeProperties : ShapePropertyCollection;
```
### isInSecondaryPlot {#isInSecondaryPlot--}
Gets or sets a value indicates whether this data points is in the second pie or bar on a pie of pie or bar of pie chart
```javascript
isInSecondaryPlot : boolean;
```
### shapeX {#shapeX--}
Readonly. Gets the x coordinate of the upper left corner in units of 1/4000 of chart's width after calls Chart.Calculate() method.
```javascript
shapeX : number;
```
### shapeY {#shapeY--}
Readonly. Gets the y coordinate of the upper left corner in units of 1/4000 of chart's height after calls Chart.Calculate() method.
```javascript
shapeY : number;
```
### shapeWidth {#shapeWidth--}
Readonly. Gets the width in units of 1/4000 of chart's width after calls Chart.Calculate() method.
```javascript
shapeWidth : number;
```
### shapeHeight {#shapeHeight--}
Readonly. Gets the height in units of 1/4000 of chart's height after calls Chart.Calculate() method.
```javascript
shapeHeight : number;
```
### shapeXPx {#shapeXPx--}
Readonly. Gets the x coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method.
```javascript
shapeXPx : number;
```
### shapeYPx {#shapeYPx--}
Readonly. Gets the y coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method.
```javascript
shapeYPx : number;
```
### shapeWidthPx {#shapeWidthPx--}
Readonly. Gets the width in units of pixels after calls Chart.Calculate() method.
```javascript
shapeWidthPx : number;
```
### shapeHeightPx {#shapeHeightPx--}
Readonly. Gets the height in units of pixels after calls Chart.Calculate() method.
```javascript
shapeHeightPx : number;
```
### borderWidthPx {#borderWidthPx--}
Readonly. Gets the width of border in units of pixels after calls Chart.Calculate() method.
```javascript
borderWidthPx : number;
```
### radiusPx {#radiusPx--}
Readonly. Gets the radius of bubble, pie or doughnut in units of pixels after calls Chart.Calculate() method.
```javascript
radiusPx : number;
```
### doughnutInnerRadius {#doughnutInnerRadius--}
Readonly. Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method. Applies to Doughnut chart.
```javascript
doughnutInnerRadius : number;
```
### innerRadiusPx {#innerRadiusPx--}
Readonly. Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method. Applies to Doughnut chart.
```javascript
innerRadiusPx : number;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use ChartPoint.DoughnutInnerRadius property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
### startAngle {#startAngle--}
Readonly. Gets the starting angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method. Applies to Pie chart.
```javascript
startAngle : number;
```
### endAngle {#endAngle--}
Readonly. Gets the ending angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method. Applies to Pie chart.
```javascript
endAngle : number;
```
### arcStartPointXPx {#arcStartPointXPx--}
Readonly. Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut  chart.
```javascript
arcStartPointXPx : number;
```
### arcStartPointYPx {#arcStartPointYPx--}
Readonly. Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut  chart.
```javascript
arcStartPointYPx : number;
```
### arcEndPointXPx {#arcEndPointXPx--}
Readonly. Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut  chart.
```javascript
arcEndPointXPx : number;
```
### arcEndPointYPx {#arcEndPointYPx--}
Readonly. Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart.
```javascript
arcEndPointYPx : number;
```
### innerArcStartPointXPx {#innerArcStartPointXPx--}
Readonly. Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart.
```javascript
innerArcStartPointXPx : number;
```
### innerArcStartPointYPx {#innerArcStartPointYPx--}
Readonly. Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart.
```javascript
innerArcStartPointYPx : number;
```
### innerArcEndPointXPx {#innerArcEndPointXPx--}
Readonly. Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart.
```javascript
innerArcEndPointXPx : number;
```
### innerArcEndPointYPx {#innerArcEndPointYPx--}
Readonly. Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart.
```javascript
innerArcEndPointYPx : number;
```
### getExplosion() {#getExplosion--}
```javascript
getExplosion() : number;
```
### setExplosion(number) {#setExplosion-number-}
```javascript
setExplosion(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getShadow() {#getShadow--}
```javascript
getShadow() : boolean;
```
### setShadow(boolean) {#setShadow-boolean-}
```javascript
setShadow(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getBorder() {#getBorder--}
```javascript
getBorder() : Line;
```
**Returns**
[Line](../line/)
### getArea() {#getArea--}
```javascript
getArea() : Area;
```
**Returns**
[Area](../area/)
### getMarker() {#getMarker--}
```javascript
getMarker() : Marker;
```
**Returns**
[Marker](../marker/)
### getDataLabels() {#getDataLabels--}
```javascript
getDataLabels() : DataLabels;
```
**Returns**
[DataLabels](../datalabels/)
### get_YValue() {#get_YValue--}
```javascript
get_YValue() : Object;
```
### setYValue(Object) {#setYValue-object-}
```javascript
setYValue(value: Object) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | The value to set. |
### getYValueType() {#getYValueType--}
```javascript
getYValueType() : CellValueType;
```
**Returns**
[CellValueType](../cellvaluetype/)
### getXValue() {#getXValue--}
```javascript
getXValue() : Object;
```
### setXValue(Object) {#setXValue-object-}
```javascript
setXValue(value: Object) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | The value to set. |
### getXValueType() {#getXValueType--}
```javascript
getXValueType() : CellValueType;
```
**Returns**
[CellValueType](../cellvaluetype/)
### getShapeProperties() {#getShapeProperties--}
```javascript
getShapeProperties() : ShapePropertyCollection;
```
**Returns**
[ShapePropertyCollection](../shapepropertycollection/)
### isInSecondaryPlot() {#isInSecondaryPlot--}
```javascript
isInSecondaryPlot() : boolean;
```
### setIsInSecondaryPlot(boolean) {#setIsInSecondaryPlot-boolean-}
```javascript
setIsInSecondaryPlot(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShapeX() {#getShapeX--}
```javascript
getShapeX() : number;
```
### getShapeY() {#getShapeY--}
```javascript
getShapeY() : number;
```
### getShapeWidth() {#getShapeWidth--}
```javascript
getShapeWidth() : number;
```
### getShapeHeight() {#getShapeHeight--}
```javascript
getShapeHeight() : number;
```
### getShapeXPx() {#getShapeXPx--}
```javascript
getShapeXPx() : number;
```
### getShapeYPx() {#getShapeYPx--}
```javascript
getShapeYPx() : number;
```
### getShapeWidthPx() {#getShapeWidthPx--}
```javascript
getShapeWidthPx() : number;
```
### getShapeHeightPx() {#getShapeHeightPx--}
```javascript
getShapeHeightPx() : number;
```
### getBorderWidthPx() {#getBorderWidthPx--}
```javascript
getBorderWidthPx() : number;
```
### getRadiusPx() {#getRadiusPx--}
```javascript
getRadiusPx() : number;
```
### getDoughnutInnerRadius() {#getDoughnutInnerRadius--}
```javascript
getDoughnutInnerRadius() : number;
```
### getInnerRadiusPx() {#getInnerRadiusPx--}
```javascript
getInnerRadiusPx() : number;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use ChartPoint.DoughnutInnerRadius property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
### getStartAngle() {#getStartAngle--}
```javascript
getStartAngle() : number;
```
### getEndAngle() {#getEndAngle--}
```javascript
getEndAngle() : number;
```
### getArcStartPointXPx() {#getArcStartPointXPx--}
```javascript
getArcStartPointXPx() : number;
```
### getArcStartPointYPx() {#getArcStartPointYPx--}
```javascript
getArcStartPointYPx() : number;
```
### getArcEndPointXPx() {#getArcEndPointXPx--}
```javascript
getArcEndPointXPx() : number;
```
### getArcEndPointYPx() {#getArcEndPointYPx--}
```javascript
getArcEndPointYPx() : number;
```
### getInnerArcStartPointXPx() {#getInnerArcStartPointXPx--}
```javascript
getInnerArcStartPointXPx() : number;
```
### getInnerArcStartPointYPx() {#getInnerArcStartPointYPx--}
```javascript
getInnerArcStartPointYPx() : number;
```
### getInnerArcEndPointXPx() {#getInnerArcEndPointXPx--}
```javascript
getInnerArcEndPointXPx() : number;
```
### getInnerArcEndPointYPx() {#getInnerArcEndPointYPx--}
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
