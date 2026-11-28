---
title: ChartPointCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a collection that contains all the points in one series.
type: docs
url: /fr/nodejs-cpp/chartpointcollection/
---

## ChartPointCollection class

Represents a collection that contains all the points in one series.

```javascript
class ChartPointCollection implements Iterable<ChartPoint>;
```


### Example
```javascript
const { Workbook, ChartType, Color } = require("aspose.cells.node");

//Instanciation d'un objet Workbook
var workbook = new Workbook();
//Obtenir la référence de la première feuille de calcul
var worksheet = workbook.worksheets.get(0);
//Ajout d'une valeur d'exemple à la cellule "A1"
worksheet.cells.get("A1").putValue(50);
//Ajout d'une valeur d'exemple à la cellule "A2"
worksheet.cells.get("A2").putValue(100);
//Ajout d'une valeur d'exemple à la cellule "A3"
worksheet.cells.get("A3").putValue(150);
//Ajout d'une valeur d'exemple à la cellule "B1"
worksheet.cells.get("B1").putValue(60);
//Ajout d'une valeur d'exemple à la cellule "B2"
worksheet.cells.get("B2").putValue(32);
//Ajout d'une valeur d'exemple à la cellule "B3"
worksheet.cells.get("B3").putValue(50);
//Ajout d'un graphique à la feuille de calcul
var chartIndex = worksheet.charts.add(ChartType.PieExploded, 5, 0, 25, 10);
//Accès à l'instance du graphique récemment ajouté
var chart = worksheet.charts.get(chartIndex);
//Ajouter NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "B3"
chart.nSeries.add("A1:B3", true);
//Afficher les étiquettes de données 
chart.nSeries.get(0).dataLabels.showValue = true;
var points = chart.nSeries.get(0).points;
var red = Color.Red;
for (var i = 0; i < points.count; i++) {
    //Obtenir le point de données
    var point = points.get(i);
    //Définir l'explosion du Pir
    point.explosion = 15;
    //Définir la couleur de bordure
    point.border.color = red;
}

//Enregistrement du fichier Excel
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



