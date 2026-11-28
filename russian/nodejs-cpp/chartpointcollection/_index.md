---
title: ChartPointCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a collection that contains all the points in one series.
type: docs
url: /ru/nodejs-cpp/chartpointcollection/
---

## ChartPointCollection class

Represents a collection that contains all the points in one series.

```javascript
class ChartPointCollection implements Iterable<ChartPoint>;
```


### Example
```javascript
const { Workbook, ChartType, Color } = require("aspose.cells.node");

//Создание объекта Workbook
var workbook = new Workbook();
//Получение ссылки на первый лист.
var worksheet = workbook.worksheets.get(0);
//Добавление примерного значения в ячейку "A1"
worksheet.cells.get("A1").putValue(50);
//Добавление примерного значения в ячейку "A2"
worksheet.cells.get("A2").putValue(100);
//Добавление примерного значения в ячейку "A3"
worksheet.cells.get("A3").putValue(150);
//Добавление примерного значения в ячейку "B1"
worksheet.cells.get("B1").putValue(60);
//Добавление примерного значения в ячейку "B2"
worksheet.cells.get("B2").putValue(32);
//Добавление примерного значения в ячейку "B3"
worksheet.cells.get("B3").putValue(50);
//Добавление диаграммы в лист
var chartIndex = worksheet.charts.add(ChartType.PieExploded, 5, 0, 25, 10);
//Получение экземпляра только что добавленной диаграммы
var chart = worksheet.charts.get(chartIndex);
//Добавление NSeries (источник данных диаграммы) к диаграмме в диапазоне от ячейки "A1" до "B3"
chart.nSeries.add("A1:B3", true);
//Показать подписи данных
chart.nSeries.get(0).dataLabels.showValue = true;
var points = chart.nSeries.get(0).points;
var red = Color.Red;
for (var i = 0; i < points.count; i++) {
    //Получить точку данных
    var point = points.get(i);
    //Установить взрыв Pir
    point.explosion = 15;
    //Установить цвет границы
    point.border.color = red;
}

//Сохранение файла Excel
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



