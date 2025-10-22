##ChartPoint
Represents a single point in a series in a chart.
## ChartPoint class
Represents a single point in a series in a chart.
```javascript
class ChartPoint;
```
### Example
```javascript
const { Workbook, ChartType, Color, SaveFormat } = AsposeCells;
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
var uint8Array = workbook.save(SaveFormat.Xlsx);
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
| [yValue](#yValue--)| VObject | Gets or sets the Y value of the chart point. |
| [yValueType](#yValueType--)| CellValueType | Readonly. Gets Y value type of the chart point. |
| [xValue](#xValue--)| VObject | Gets or sets the X value of the chart point. |
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
| [getTopPointCount()](#getTopPointCount--)| Gets the number of top points after calls Chart.Calculate() method. |
| [getTopPointXPx(number)](#getTopPointXPx-number-)| Gets x-coordinate of the top point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid and Area3D |
| [getTopPointYPx(number)](#getTopPointYPx-number-)| Gets y-coordinate of the top point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid and Area3D |
| [getBottomPointCount()](#getBottomPointCount--)| Gets the number of bottom points  after calls Chart.Calculate() method. |
| [getBottomPointXPx(number)](#getBottomPointXPx-number-)| Gets x-coordinate of the bottom point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid |
| [getBottomPointYPx(number)](#getBottomPointYPx-number-)| Gets y-coordinate of the bottom point of shape  after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid |
| [getOnCategoryAxisPointCount()](#getOnCategoryAxisPointCount--)| Gets the number of the points on category axis after calls Chart.Calculate() method. Only applies to area chart. |
| [getOnCategoryAxisPointXPx(number)](#getOnCategoryAxisPointXPx-number-)| Gets x-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart. |
| [getOnCategoryAxisPointYPx(number)](#getOnCategoryAxisPointYPx-number-)| Gets y-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart. |
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
yValue : VObject;
```
### yValueType {#yValueType--}
Readonly. Gets Y value type of the chart point.
```javascript
yValueType : CellValueType;
```
### xValue {#xValue--}
Gets or sets the X value of the chart point.
```javascript
xValue : VObject;
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
