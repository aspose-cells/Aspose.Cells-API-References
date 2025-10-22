##TrendlineCollection
Represents a collection of all the Trendline..trendline objects for the specified data series.
## TrendlineCollection class
Represents a collection of all the [Trendline](../trendline/) objects for the specified data series.
```javascript
class TrendlineCollection;
```
### Example
```javascript
const { Workbook, ChartType, TrendlineType, Color } = require("aspose.cells.node");
var excel = new Workbook();
var chartIndex = excel.worksheets.get(0).charts.add(ChartType.Column, 3, 3, 15, 10);
var chart = excel.worksheets.get(0).charts.get(chartIndex);
chart.nSeries.add("A1:a3", true);
chart.nSeries.get(0).trendLines.add(TrendlineType.Linear, "MyTrendLine");
var line = chart.nSeries.get(0).trendLines.get(0);
line.displayEquation = true;
line.displayRSquared = true;
line.color = Color.Red;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets a [Trendline](../trendline/) object by its index. |
| [add(TrendlineType)](#add-trendlinetype-)| Adds a [Trendline](../trendline/) object to this collection with specified type. |
| [add(TrendlineType, string)](#add-trendlinetype-string-)| Adds a [Trendline](../trendline/) object to this collection with specified type and name. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Gets a [Trendline](../trendline/) object by its index.
```javascript
get(index: number) : Trendline;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |
**Returns**
[Trendline](../trendline/)
### add(TrendlineType) {#add-trendlinetype-}
Adds a [Trendline](../trendline/) object to this collection with specified type.
```javascript
add(type: TrendlineType) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [TrendlineType](../trendlinetype/) | Trendline type. |
**Returns**
[Trendline](../trendline/) object index.
### add(TrendlineType, string) {#add-trendlinetype-string-}
Adds a [Trendline](../trendline/) object to this collection with specified type and name.
```javascript
add(type: TrendlineType, name: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [TrendlineType](../trendlinetype/) | Trendline type. |
| name | string | Trendline name. |
**Returns**
[Trendline](../trendline/) object index.
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
