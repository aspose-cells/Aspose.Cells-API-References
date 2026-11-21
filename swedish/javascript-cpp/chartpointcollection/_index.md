---
title: ChartPointCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents a collection that contains all the points in one series.
type: docs
url: /sv/javascript-cpp/chartpointcollection/
---

## ChartPointCollection class

Represents a collection that contains all the points in one series.

```javascript
class ChartPointCollection;
```


### Example
```javascript
const { Workbook, ChartType, Color, SaveFormat } = AsposeCells;

//Instansiering av ett Workbook-objekt
var workbook = new Workbook();
//Hämtar referensen till det första kalkylbladet
var worksheet = workbook.worksheets.get(0);
//Lägger till ett exempelvärde i cellen "A1"
worksheet.cells.get("A1").putValue(50);
//Lägger till ett exempelvärde i cellen "A2"
worksheet.cells.get("A2").putValue(100);
//Lägger till ett exempelvärde i cellen "A3"
worksheet.cells.get("A3").putValue(150);
//Lägger till ett exempelvärde i cellen "B1"
worksheet.cells.get("B1").putValue(60);
//Lägger till ett exempelvärde i cellen "B2"
worksheet.cells.get("B2").putValue(32);
//Lägger till ett exempelvärde i cellen "B3"
worksheet.cells.get("B3").putValue(50);
//Lägger till ett diagram i kalkylbladet
var chartIndex = worksheet.charts.add(ChartType.PieExploded, 5, 0, 25, 10);
//Åtkomst till instansen av det nyss tillagda diagrammet
var chart = worksheet.charts.get(chartIndex);
//Lägger till NSeries (diagramdatakälla) i diagrammet från cell "A1" till "B3"
chart.nSeries.add("A1:B3", true);
//Visa datamärkningar
chart.nSeries.get(0).dataLabels.showValue = true;
var points = chart.nSeries.get(0).points;
var red = Color.Red;
for (var i = 0; i < points.count; i++) {
    //Hämta datapunkt
    var point = points.get(i);
    //Ställ in Pir-explosion
    point.explosion = 15;
    //Ställ in kantfärg
    point.border.color = red;
}

//Sparar Excel-filen
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Properties

| Property | Type | Description |
| --- | --- | --- |
| [count](#count--)| number | Readonly. Gets the count of the chart point. |

## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [ChartPoint](../chartpoint/) element at the specified index in the series. |
| [getEnumerator()](#getEnumerator--)| Returns an enumerator for the entire [ChartPointCollection](../chartpointcollection/). |
| [clear()](#clear--)| Remove all setting of the chart points. |
| [removeAt(number)](#removeAt-number-)| Removes point at the index of the series. |


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


