##ChartPointCollection
Represents a collection that contains all the points in one series.
## ChartPointCollection class
Represents a collection that contains all the points in one series.
```javascript
class ChartPointCollection;
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
var points = chart.nSeries.get(0).points;
var red = Color.Red;
for (var i = 0; i < points.count; i++) {
//Get Data Point
var point = points.get(i);
//Set Pir Explosion
point.explosion = 15;
//Set Border Color
point.border.color = red;
}
//Saving the Excel file
workbook.save("output/ChartsChartPointCollection.xls");
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [count](#count--)| number | Readonly. Gets the count of the chart point. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [ChartPoint](../chartpoint/) element at the specified index in the series. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the count of the chart point. |
| [getEnumerator()](#getEnumerator--)| Returns an enumerator for the entire [ChartPointCollection](../chartpointcollection/). |
| [clear()](#clear--)| Remove all setting of the chart points. |
| [removeAt(number)](#removeAt-number-)| Removes point at the index of the series.. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### count {#count--}
Readonly. Gets the count of the chart point.
```javascript
count : number;
```
### get(number) {#get-number-}
Gets the [ChartPoint](../chartpoint/) element at the specified index in the series.
```javascript
get(index: number) : ChartPoint;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index of chart point in the series. |
**Returns**
The ChartPoint object.
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### getEnumerator() {#getEnumerator--}
Returns an enumerator for the entire [ChartPointCollection](../chartpointcollection/).
```javascript
getEnumerator() : ChartPointEnumerator;
```
**Returns**
[ChartPointEnumerator](../chartpointenumerator/)
### clear() {#clear--}
Remove all setting of the chart points.
```javascript
clear() : void;
```
### removeAt(number) {#removeAt-number-}
Removes point at the index of the series..
```javascript
removeAt(index: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index of the point. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
