---
title: ChartPointCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a collection that contains all the points in one series.
type: docs
url: /es/nodejs-cpp/chartpointcollection/
---

## ChartPointCollection class

Represents a collection that contains all the points in one series.

```javascript
class ChartPointCollection implements Iterable<ChartPoint>;
```


### Example
```javascript
const { Workbook, ChartType, Color } = require("aspose.cells.node");

//Instanciando un objeto Workbook
var workbook = new Workbook();
//Obtener la referencia de la primera hoja de cálculo
var worksheet = workbook.worksheets.get(0);
//Añadiendo un valor de ejemplo a la celda "A1"
worksheet.cells.get("A1").putValue(50);
//Añadiendo un valor de ejemplo a la celda "A2"
worksheet.cells.get("A2").putValue(100);
//Añadiendo un valor de ejemplo a la celda "A3"
worksheet.cells.get("A3").putValue(150);
//Añadiendo un valor de ejemplo a la celda "B1"
worksheet.cells.get("B1").putValue(60);
//Añadiendo un valor de ejemplo a la celda "B2"
worksheet.cells.get("B2").putValue(32);
//Añadiendo un valor de ejemplo a la celda "B3"
worksheet.cells.get("B3").putValue(50);
//Agregar un gráfico a la hoja de cálculo
var chartIndex = worksheet.charts.add(ChartType.PieExploded, 5, 0, 25, 10);
//Accediendo a la instancia del gráfico recién agregado
var chart = worksheet.charts.get(chartIndex);
//Agregar NSeries (fuente de datos del gráfico) al gráfico que abarca desde la celda "A1" hasta "B3"
chart.nSeries.add("A1:B3", true);
//Mostrar etiquetas de datos
chart.nSeries.get(0).dataLabels.showValue = true;
var points = chart.nSeries.get(0).points;
var red = Color.Red;
for (var i = 0; i < points.count; i++) {
    //Obtener punto de datos
    var point = points.get(i);
    //Establecer explosión Pir
    point.explosion = 15;
    //Establecer color del borde
    point.border.color = red;
}

//Guardando el archivo Excel
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



