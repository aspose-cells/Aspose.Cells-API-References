---
title: SeriesCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates a collection of Series..series objects.
type: docs
url: /zh/nodejs-cpp/seriescollection/
---

## SeriesCollection class

Encapsulates a collection of [Series](../series/) objects.

```javascript
class SeriesCollection implements Iterable<Series>;
```


### Example
```javascript
const { Workbook, ChartType } = require("aspose.cells.node");

//实例化一个 Workbook 对象
var workbook = new Workbook();
//向 Excel 对象添加新工作表
var sheetIndex = workbook.worksheets.add();
//通过传递工作表索引获取新添加工作表的引用
var worksheet = workbook.worksheets.get(sheetIndex);
//向 "A1" 单元格添加示例值
worksheet.cells.get("A1").putValue(50);
//向 "A2" 单元格添加示例值
worksheet.cells.get("A2").putValue(100);
//向 "A3" 单元格添加示例值
worksheet.cells.get("A3").putValue(150);
//向 "A4" 单元格添加示例值
worksheet.cells.get("A4").putValue(200);
//向 "B1" 单元格添加示例值
worksheet.cells.get("B1").putValue(60);
//向 "B2" 单元格添加示例值
worksheet.cells.get("B2").putValue(32);
//向 "B3" 单元格添加示例值
worksheet.cells.get("B3").putValue(50);
//向 "B4" 单元格添加示例值
worksheet.cells.get("B4").putValue(40);
//向 "C1" 单元格添加示例值作为类别数据
worksheet.cells.get("C1").putValue("Q1");
//向 "C2" 单元格添加示例值作为类别数据
worksheet.cells.get("C2").putValue("Q2");
//将示例值添加到 "C3" 单元格作为类别数据
worksheet.cells.get("C3").putValue("Y1");
//将示例值添加到 "C4" 单元格作为类别数据
worksheet.cells.get("C4").putValue("Y2");
//向工作表添加图表
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//访问新添加图表的实例
var chart = worksheet.charts.get(chartIndex);
//将 NSeries（图表数据源）添加到范围为 "A1" 单元格到 "B4" 的图表中
chart.nSeries.add("A1:B4", true);
//设置 NSeries 类别数据的数据源
chart.nSeries.categoryData = "C1:C4";
//保存 Excel 文件
workbook.save("output/ChartsSeriesCollection.xls");
```
## Properties

| Property | Type | Description |
| --- | --- | --- |
| [categoryData](#categoryData--)| string | Gets or sets the range of category Axis values. It can be a range of cells (such as "d1:e10") or a sequence of values (such as "{2,6,8,10}"). |
| [secondCategoryData](#secondCategoryData--)| string | Gets or sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some series were plotted on the second axis. |
| [isColorVaried](#isColorVaried--)| boolean | Represents if the color of points is varied. |

## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [Series](../series/) element at the specified index. |
| [getCategoryData()](#getCategoryData--)| <b>@deprecated.</b> Please use the 'categoryData' property instead. Gets or sets the range of category Axis values. It can be a range of cells (such as "d1:e10") or a sequence of values (such as "{2,6,8,10}"). |
| [setCategoryData(string)](#setCategoryData-string-)| <b>@deprecated.</b> Please use the 'categoryData' property instead. Gets or sets the range of category Axis values. It can be a range of cells (such as "d1:e10") or a sequence of values (such as "{2,6,8,10}"). |
| [getSecondCategoryData()](#getSecondCategoryData--)| <b>@deprecated.</b> Please use the 'secondCategoryData' property instead. Gets or sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some series were plotted on the second axis. |
| [setSecondCategoryData(string)](#setSecondCategoryData-string-)| <b>@deprecated.</b> Please use the 'secondCategoryData' property instead. Gets or sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some series were plotted on the second axis. |
| [isColorVaried()](#isColorVaried--)| <b>@deprecated.</b> Please use the 'isColorVaried' property instead. Represents if the color of points is varied. |
| [setIsColorVaried(boolean)](#setIsColorVaried-boolean-)| <b>@deprecated.</b> Please use the 'isColorVaried' property instead. Represents if the color of points is varied. |
| [getSeriesByOrder(number)](#getSeriesByOrder-number-)| Gets the [Series](../series/) element by order. |
| [removeAt(number)](#removeAt-number-)| Remove at a series at the specific index. |
| [changeSeriesOrder(number, number)](#changeSeriesOrder-number-number-)| Directly changes the orders of the two series. |
| [swapSeries(number, number)](#swapSeries-number-number-)| Directly changes the orders of the two series. |
| [setSeriesNames(number, string, boolean)](#setSeriesNames-number-string-boolean-)| Sets the names of all the series in the chart. |
| [addR1C1(string, boolean)](#addR1C1-string-boolean-)| Adds the [Series](../series/) collection to a chart. |
| [add(string, boolean)](#add-string-boolean-)| Adds the [Series](../series/) collection to a chart. |
| [add(string, boolean, boolean)](#add-string-boolean-boolean-)| Adds the [Series](../series/) collection to a chart. |
| [clear()](#clear--)| Clears the collection |
| [changeColors(ChartColorPaletteType)](#changeColors-chartcolorpalettetype-)| Set Monochromatic Palette for chart series. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |

## \[Symbol.iterator\](): Iterator\<Series\>

Returns an iterator over the items in the collection. Enables use of `for...of`, spread syntax, and `Array.from()`.



### categoryData {#categoryData--}

Gets or sets the range of category Axis values. It can be a range of cells (such as "d1:e10") or a sequence of values (such as "{2,6,8,10}").

```javascript
categoryData : string;
```


### secondCategoryData {#secondCategoryData--}

Gets or sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some series were plotted on the second axis.

```javascript
secondCategoryData : string;
```


### isColorVaried {#isColorVaried--}

Represents if the color of points is varied.

```javascript
isColorVaried : boolean;
```


**Remarks**

Only works for pie chart or when there is only one series.

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

<b>@deprecated.</b> Please use the 'categoryData' property instead. Gets or sets the range of category Axis values. It can be a range of cells (such as "d1:e10") or a sequence of values (such as "{2,6,8,10}").

```javascript
getCategoryData() : string;
```


### setCategoryData(string) {#setCategoryData-string-}

<b>@deprecated.</b> Please use the 'categoryData' property instead. Gets or sets the range of category Axis values. It can be a range of cells (such as "d1:e10") or a sequence of values (such as "{2,6,8,10}").

```javascript
setCategoryData(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getSecondCategoryData() {#getSecondCategoryData--}

<b>@deprecated.</b> Please use the 'secondCategoryData' property instead. Gets or sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some series were plotted on the second axis.

```javascript
getSecondCategoryData() : string;
```


### setSecondCategoryData(string) {#setSecondCategoryData-string-}

<b>@deprecated.</b> Please use the 'secondCategoryData' property instead. Gets or sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some series were plotted on the second axis.

```javascript
setSecondCategoryData(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isColorVaried() {#isColorVaried--}

<b>@deprecated.</b> Please use the 'isColorVaried' property instead. Represents if the color of points is varied.

```javascript
isColorVaried() : boolean;
```


**Remarks**

Only works for pie chart or when there is only one series.

### setIsColorVaried(boolean) {#setIsColorVaried-boolean-}

<b>@deprecated.</b> Please use the 'isColorVaried' property instead. Represents if the color of points is varied.

```javascript
setIsColorVaried(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only works for pie chart or when there is only one series.

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

Sets the names of all the series in the chart.

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

br>If the start index is larger than the count of the serieses, it will return and do nothing.</br> <br>If set data on contiguous cells, use colon to separate them. For example, $C$2:$C$5.</br> <br>If set data on contiguous cells, use comma to separate them. For example, ($C$2,$D$5).</br

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

br>If set data on contiguous cells, use colon to separate them. For example, R[1]C[1]:R[3]C[2].</br> <br>If set data on contiguous cells, use comma to separate them. For example,(R[1]C[1],R[3]C[2]).</br

### add(string, boolean) {#add-string-boolean-}

Adds the [Series](../series/) collection to a chart.

```javascript
add(dataArea: string, isVertical: boolean) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dataArea | string | Specifies values from which to plot the data series |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column.         /// If true, [Series](../series/) will be added column by column |

**Returns**

Return the first index of the added ASeries in the NSeries.

**Remarks**

br>If set data on contiguous cells, use colon to separate them.For example, $C$2:$C$5.</br> <br>If set data on non contiguous cells, use comma to separate them.For example: ($C$2,$D$5).</br> <br>This method only simply process <paramref name="dataArea"/> as data range. If you want to smartly check ChartCollection.Add() method. </br

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

br>If set data on contiguous cells, use colon to separate them. For example, $C$2:$C$5.</br> <br>If set data on non contiguous cells, use comma to separate them. For example, ($C$2,$D$5).</br

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

<b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in.

```javascript
getCount() : number;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



