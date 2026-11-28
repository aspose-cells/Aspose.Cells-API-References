---
title: ChartPointCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a collection that contains all the points in one series.
type: docs
url: /zh/nodejs-cpp/chartpointcollection/
---

## ChartPointCollection class

Represents a collection that contains all the points in one series.

```javascript
class ChartPointCollection implements Iterable<ChartPoint>;
```


### Example
```javascript
const { Workbook, ChartType, Color } = require("aspose.cells.node");

//实例化一个 Workbook 对象
var workbook = new Workbook();
//获取第一个工作表的引用
var worksheet = workbook.worksheets.get(0);
//向 "A1" 单元格添加示例值
worksheet.cells.get("A1").putValue(50);
//向 "A2" 单元格添加示例值
worksheet.cells.get("A2").putValue(100);
//向 "A3" 单元格添加示例值
worksheet.cells.get("A3").putValue(150);
//向 "B1" 单元格添加示例值
worksheet.cells.get("B1").putValue(60);
//向 "B2" 单元格添加示例值
worksheet.cells.get("B2").putValue(32);
//向 "B3" 单元格添加示例值
worksheet.cells.get("B3").putValue(50);
//向工作表添加图表
var chartIndex = worksheet.charts.add(ChartType.PieExploded, 5, 0, 25, 10);
//访问新添加图表的实例
var chart = worksheet.charts.get(chartIndex);
//向图表添加 NSeries（图表数据源），范围从 "A1" 单元格到 "B3"
chart.nSeries.add("A1:B3", true);
//显示数据标签
chart.nSeries.get(0).dataLabels.showValue = true;
var points = chart.nSeries.get(0).points;
var red = Color.Red;
for (var i = 0; i < points.count; i++) {
    //获取数据点
    var point = points.get(i);
    //设置 Pir 爆炸
    point.explosion = 15;
    //设置边框颜色
    point.border.color = red;
}

//保存 Excel 文件
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
| [removeAt(number)](#removeAt-number-)| Removes point at the index of the series. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |

## \[Symbol.iterator\](): Iterator\<ChartPoint\>

Returns an iterator over the items in the collection. Enables use of `for...of`, spread syntax, and `Array.from()`.



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

<b>@deprecated.</b> Please use the 'count' property instead. Gets the count of the chart point.

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

Removes point at the index of the series.

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



