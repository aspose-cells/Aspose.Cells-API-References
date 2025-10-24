##SeriesCollection
Encapsulates a collection of Series..series objects.
## SeriesCollection class
Encapsulates a collection of [Series](../series/) objects.
```javascript
class SeriesCollection;
```
### Example
```javascript
const { Workbook, ChartType } = require("aspose.cells.node");
//Instantiating a Workbook object
var workbook = new Workbook();
//Adding a new worksheet to the Excel object
var sheetIndex = workbook.worksheets.add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
var worksheet = workbook.worksheets.get(sheetIndex);
//Adding a sample value to "A1" cell
worksheet.cells.get("A1").putValue(50);
//Adding a sample value to "A2" cell
worksheet.cells.get("A2").putValue(100);
//Adding a sample value to "A3" cell
worksheet.cells.get("A3").putValue(150);
//Adding a sample value to "A4" cell
worksheet.cells.get("A4").putValue(200);
//Adding a sample value to "B1" cell
worksheet.cells.get("B1").putValue(60);
//Adding a sample value to "B2" cell
worksheet.cells.get("B2").putValue(32);
//Adding a sample value to "B3" cell
worksheet.cells.get("B3").putValue(50);
//Adding a sample value to "B4" cell
worksheet.cells.get("B4").putValue(40);
//Adding a sample value to "C1" cell as category data
worksheet.cells.get("C1").putValue("Q1");
//Adding a sample value to "C2" cell as category data
worksheet.cells.get("C2").putValue("Q2");
//Adding a sample value to "C3" cell as category data
worksheet.cells.get("C3").putValue("Y1");
//Adding a sample value to "C4" cell as category data
worksheet.cells.get("C4").putValue("Y2");
//Adding a chart to the worksheet
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//Accessing the instance of the newly added chart
var chart = worksheet.charts.get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.nSeries.add("A1:B4", true);
//Setting the data source for the category data of NSeries
chart.nSeries.categoryData = "C1:C4";
//Saving the Excel file
workbook.save("output/ChartsSeriesCollection.xls");
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [categoryData](#categoryData--)| string | Gets or sets the range of category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). |
| [secondCategoryData](#secondCategoryData--)| string | Gets or sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some ASerieses plot on the second axis. |
| [isColorVaried](#isColorVaried--)| boolean | Represents if the color of points is varied. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [Series](../series/) element at the specified index. |
| [getCategoryData()](#getCategoryData--)| <b>@deprecated.</b> Please use the 'categoryData' property instead. Gets or sets the range of category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). |
| [setCategoryData(string)](#setCategoryData-string-)| <b>@deprecated.</b> Please use the 'categoryData' property instead. Gets or sets the range of category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). |
| [getSecondCategoryData()](#getSecondCategoryData--)| <b>@deprecated.</b> Please use the 'secondCategoryData' property instead. Gets or sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some ASerieses plot on the second axis. |
| [setSecondCategoryData(string)](#setSecondCategoryData-string-)| <b>@deprecated.</b> Please use the 'secondCategoryData' property instead. Gets or sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some ASerieses plot on the second axis. |
| [isColorVaried()](#isColorVaried--)| <b>@deprecated.</b> Please use the 'isColorVaried' property instead. Represents if the color of points is varied. |
| [setIsColorVaried(boolean)](#setIsColorVaried-boolean-)| <b>@deprecated.</b> Please use the 'isColorVaried' property instead. Represents if the color of points is varied. |
| [getSeriesByOrder(number)](#getSeriesByOrder-number-)| Gets the [Series](../series/) element by order. |
| [removeAt(number)](#removeAt-number-)| Remove at a series at the specific index. |
| [changeSeriesOrder(number, number)](#changeSeriesOrder-number-number-)| Directly changes the orders of the two series. |
| [swapSeries(number, number)](#swapSeries-number-number-)| Directly changes the orders of the two series. |
| [setSeriesNames(number, string, boolean)](#setSeriesNames-number-string-boolean-)| Sets the name of all the serieses in the chart. |
| [addR1C1(string, boolean)](#addR1C1-string-boolean-)| Adds the [Series](../series/) collection to a chart. |
| [add(string, boolean)](#add-string-boolean-)| Adds the [Series](../series/) collection to a chart. |
| [add(string, boolean, boolean)](#add-string-boolean-boolean-)| Adds the [Series](../series/) collection to a chart. |
| [clear()](#clear--)| Clears the collection |
| [changeColors(ChartColorPaletteType)](#changeColors-chartcolorpalettetype-)| Set Monochromatic Palette for chart series. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### categoryData {#categoryData--}
Gets or sets the range of category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}").
```javascript
categoryData : string;
```
### secondCategoryData {#secondCategoryData--}
Gets or sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some ASerieses plot on the second axis.
```javascript
secondCategoryData : string;
```
### isColorVaried {#isColorVaried--}
Represents if the color of points is varied.
```javascript
isColorVaried : boolean;
```
### get(number) {#get-number-}
Gets the [Series](../series/) element at the specified index.
```javascript
get(index: number) : Series;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |
**Returns**
The element at the specified index.
### getCategoryData() {#getCategoryData--}
```javascript
getCategoryData() : string;
```
### setCategoryData(string) {#setCategoryData-string-}
```javascript
setCategoryData(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getSecondCategoryData() {#getSecondCategoryData--}
```javascript
getSecondCategoryData() : string;
```
### setSecondCategoryData(string) {#setSecondCategoryData-string-}
```javascript
setSecondCategoryData(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### isColorVaried() {#isColorVaried--}
```javascript
isColorVaried() : boolean;
```
### setIsColorVaried(boolean) {#setIsColorVaried-boolean-}
```javascript
setIsColorVaried(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getSeriesByOrder(number) {#getSeriesByOrder-number-}
Gets the [Series](../series/) element by order.
```javascript
getSeriesByOrder(order: number) : Series;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| order | number | The order of series |
**Returns**
The element series
### removeAt(number) {#removeAt-number-}
Remove at a series at the specific index.
```javascript
removeAt(index: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
### changeSeriesOrder(number, number) {#changeSeriesOrder-number-number-}
Directly changes the orders of the two series.
```javascript
changeSeriesOrder(sourceIndex: number, destIndex: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceIndex | number | The current index |
| destIndex | number | The dest index |
**Remarks**
NOTE: This method is now obsolete. Instead, please use SeriesCollection.SwapSeries method. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
### swapSeries(number, number) {#swapSeries-number-number-}
Directly changes the orders of the two series.
```javascript
swapSeries(sourceIndex: number, destIndex: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceIndex | number | The current index |
| destIndex | number | The dest index |
### setSeriesNames(number, string, boolean) {#setSeriesNames-number-string-boolean-}
Sets the name of all the serieses in the chart.
```javascript
setSeriesNames(startIndex: number, area: string, isVertical: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | number | The index of the first series which you want to set the name. |
| area | string | Specifies the area for the series name. |
| isVertical | boolean | >Specifies whether to plot the series from a range of cell values by row or by column. |
**Remarks**
br>If the start index is larger than the count of the serieses, it will return and do nothing.</br> <br>If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5.</br> <br>If set data on contiguous cells, use comma to seperate them.For example, ($C$2,$D$5).</br
### addR1C1(string, boolean) {#addR1C1-string-boolean-}
Adds the [Series](../series/) collection to a chart.
```javascript
addR1C1(area: string, isVertical: boolean) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| area | string | Specifies values from which to plot the data series |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
**Returns**
Return the first index of the added ASeries in the NSeries.
**Remarks**
br>If set data on contiguous cells, use colon to seperate them.For example, R[1]C[1]:R[3]C[2].</br> <br>If set data on contiguous cells, use comma to seperate them.For example,(R[1]C[1],R[3]C[2]).</br
### add(string, boolean) {#add-string-boolean-}
Adds the [Series](../series/) collection to a chart.
```javascript
add(area: string, isVertical: boolean) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| area | string | Specifies values from which to plot the data series |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
**Returns**
Return the first index of the added ASeries in the NSeries.
**Remarks**
br>If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5.</br> <br>If set data on non contiguous cells, use comma to seperate them.For example: ($C$2,$D$5).</br
### add(string, boolean, boolean) {#add-string-boolean-boolean-}
Adds the [Series](../series/) collection to a chart.
```javascript
add(area: string, isVertical: boolean, checkLabels: boolean) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| area | string | Specifies values from which to plot the data series |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
| checkLabels | boolean | Indicates whether the range contains series's name |
**Returns**
Return the first index of the added ASeries in the NSeries.
**Remarks**
br>If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5.</br> <br>If set data on non contiguous cells, use comma to seperate them.For example, ($C$2,$D$5).</br
### clear() {#clear--}
Clears the collection
```javascript
clear() : void;
```
### changeColors(ChartColorPaletteType) {#changeColors-chartcolorpalettetype-}
Set Monochromatic Palette for chart series.
```javascript
changeColors(type: ChartColorPaletteType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [ChartColorPaletteType](../chartcolorpalettetype/) | The Monochromatic Type. |
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
