---
title: Area
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates the object that represents an area format.
type: docs
url: /tr/javascript-cpp/area/
---

## Area class

Encapsulates the object that represents an area format.

```javascript
class Area;
```


### Example
```javascript
const { Workbook, ChartType, Color, SaveFormat } = AsposeCells;

//Bir Workbook nesnesi oluşturma
var workbook = new Workbook();
//Workbook nesnesine yeni bir çalışma sayfası ekleme
var sheetIndex = workbook.worksheets.add();
//Yeni eklenen çalışma sayfasının referansını, sayfa indeksini geçirerek elde etme
var worksheet = workbook.worksheets.get(sheetIndex);
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
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//Yeni eklenen grafiğin örneğine erişme
var chart = worksheet.charts.get(chartIndex);
//Grafiğe "A1" hücresinden "B3" hücresine kadar NSeries (grafik veri kaynağı) ekleme
chart.nSeries.add("A1:B3", true);
//Grafik alanının ön plan rengini ayarlama
chart.plotArea.getArea().foregroundColor = Color.Blue;
//Grafik alanının ön plan rengini ayarlama
chart.chartArea.getArea().foregroundColor = Color.Yellow;
//1. NSeries alanının ön plan rengini ayarlama
chart.nSeries.get(0).area.foregroundColor = Color.Red;
//1. NSeries noktasının alanının ön plan rengini ayarlama
chart.nSeries.get(0).points.get(0).area.foregroundColor = Color.Cyan;
//Excel dosyasını kaydetme
var uint8Array = workbook.save(SaveFormat.Excel97To2003);
```
## Properties

| Property | Type | Description |
| --- | --- | --- |
| [backgroundColor](#backgroundColor--)| Color | Gets or sets the background [Color](../color/) of the [Area](../area/). |
| [foregroundColor](#foregroundColor--)| Color | Gets or sets the foreground [Color](../color/). |
| [formatting](#formatting--)| FormattingType | Represents the formatting of the area. |
| [invertIfNegative](#invertIfNegative--)| boolean | If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [fillFormat](#fillFormat--)| FillFormat | Readonly. Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape. |
| [transparency](#transparency--)| number | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |


### backgroundColor {#backgroundColor--}

Gets or sets the background [Color](../color/) of the [Area](../area/).

```javascript
backgroundColor : Color;
```


### foregroundColor {#foregroundColor--}

Gets or sets the foreground [Color](../color/).

```javascript
foregroundColor : Color;
```


### formatting {#formatting--}

Represents the formatting of the area.

```javascript
formatting : FormattingType;
```


### invertIfNegative {#invertIfNegative--}

If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```javascript
invertIfNegative : boolean;
```


**Example**
```javascript
const { Workbook, ChartType, Color, SaveFormat } = AsposeCells;

//Bir Workbook nesnesi oluşturma
var workbook = new Workbook();
//Workbook nesnesine yeni bir çalışma sayfası ekleme
var sheetIndex = workbook.worksheets.add();
//Yeni eklenen çalışma sayfasının referansını, sayfa indeksini geçirerek elde etme
var worksheet = workbook.worksheets.get(sheetIndex);
//"A1" hücresine örnek bir değer ekleme
worksheet.cells.get("A1").putValue(50);
//"A2" hücresine örnek bir değer ekleme
worksheet.cells.get("A2").putValue(-100);
//"A3" hücresine örnek bir değer ekleme
worksheet.cells.get("A3").putValue(150);
//Çalışma sayfasına bir grafik ekleme
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//Yeni eklenen grafiğin örneğine erişme
var chart = worksheet.charts.get(chartIndex);
//Grafiğe "A1" hücresinden "A3" hücresine kadar NSeries (grafik veri kaynağı) ekleme
chart.nSeries.add("A1:A3", true);
chart.nSeries.get(0).area.invertIfNegative = true;
//1. NSeries alanının ön plan rengini ayarlama
chart.nSeries.get(0).area.foregroundColor = Color.Red;
//1. NSeries alanının arka plan rengini ayarlama.
//İkinci grafik noktasının gösterilen alan rengi arka plan rengi olacaktır.
chart.nSeries.get(0).area.backgroundColor = Color.Yellow;
//Excel dosyasını kaydetme
var uint8Array = workbook.save(SaveFormat.Excel97To2003);
```

### fillFormat {#fillFormat--}

Readonly. Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape.

```javascript
fillFormat : FillFormat;
```


### transparency {#transparency--}

Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

```javascript
transparency : number;
```



