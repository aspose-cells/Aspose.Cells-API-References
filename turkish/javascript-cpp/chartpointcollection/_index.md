---
title: ChartPointCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents a collection that contains all the points in one series.
type: docs
url: /tr/javascript-cpp/chartpointcollection/
---

## ChartPointCollection class

Represents a collection that contains all the points in one series.

```javascript
class ChartPointCollection;
```


### Example
```javascript
const { Workbook, ChartType, Color, SaveFormat } = AsposeCells;

//Bir Workbook nesnesi oluşturma
var workbook = new Workbook();
//İlk çalışma sayfasının referansını elde etme
var worksheet = workbook.worksheets.get(0);
//"A1" hücresine örnek bir değer ekleme
worksheet.cells.get("A1").putValue(50);
//"A2" hücresine örnek bir değer ekleme
worksheet.cells.get("A2").putValue(100);
//"A3" hücresine örnek bir değer ekleme
worksheet.cells.get("A3").putValue(150);
//"B1" hücresine örnek bir değer ekleme
worksheet.cells.get("B1").putValue(60);
//"B2" hücresine örnek bir değer ekleme
worksheet.cells.get("B2").putValue(32);
//"B3" hücresine örnek bir değer ekleme
worksheet.cells.get("B3").putValue(50);
//Çalışma sayfasına bir grafik ekleme
var chartIndex = worksheet.charts.add(ChartType.PieExploded, 5, 0, 25, 10);
//Yeni eklenen grafiğin örneğine erişme
var chart = worksheet.charts.get(chartIndex);
//Grafiğe "A1" hücresinden "B3" hücresine kadar NSeries (grafik veri kaynağı) ekleme
chart.nSeries.add("A1:B3", true);
//Veri Etiketlerini Göster
chart.nSeries.get(0).dataLabels.showValue = true;
var points = chart.nSeries.get(0).points;
var red = Color.Red;
for (var i = 0; i < points.count; i++) {
    //Veri Noktasını Al
    var point = points.get(i);
    //Pir Patlamasını ayarla
    point.explosion = 15;
    //Kenarlık Rengini ayarla
    point.border.color = red;
}

//Excel dosyasını kaydetme
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


