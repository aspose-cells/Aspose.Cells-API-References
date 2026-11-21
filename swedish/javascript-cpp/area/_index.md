---
title: Area
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates the object that represents an area format.
type: docs
url: /sv/javascript-cpp/area/
---

## Area class

Encapsulates the object that represents an area format.

```javascript
class Area;
```


### Example
```javascript
const { Workbook, ChartType, Color, SaveFormat } = AsposeCells;

//Instansiering av ett Workbook-objekt
var workbook = new Workbook();
//Lägger till ett nytt arbetsblad i Workbook-objektet
var sheetIndex = workbook.worksheets.add();
//Hämtar referensen till det nyss tillagda kalkylbladet genom att skicka dess bladindex
var worksheet = workbook.worksheets.get(sheetIndex);
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
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//Åtkomst till instansen av det nyss tillagda diagrammet
var chart = worksheet.charts.get(chartIndex);
//Lägger till NSeries (diagramdatakälla) i diagrammet från cell "A1" till "B3"
chart.nSeries.add("A1:B3", true);
//Ställer in förgrundsfärgen för plotområdet
chart.plotArea.getArea().foregroundColor = Color.Blue;
//Ställer in förgrundsfärgen för diagramområdet
chart.chartArea.getArea().foregroundColor = Color.Yellow;
//Ställer in förgrundsfärgen för det första NSeries-området
chart.nSeries.get(0).area.foregroundColor = Color.Red;
//Ställer in förgrundsfärgen för området för den första NSeries-punkten
chart.nSeries.get(0).points.get(0).area.foregroundColor = Color.Cyan;
//Sparar Excel-filen
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

//Instansiering av ett Workbook-objekt
var workbook = new Workbook();
//Lägger till ett nytt arbetsblad i Workbook-objektet
var sheetIndex = workbook.worksheets.add();
//Hämtar referensen till det nyss tillagda kalkylbladet genom att skicka dess bladindex
var worksheet = workbook.worksheets.get(sheetIndex);
//Lägger till ett exempelvärde i cellen "A1"
worksheet.cells.get("A1").putValue(50);
//Lägger till ett exempelvärde i cellen "A2"
worksheet.cells.get("A2").putValue(-100);
//Lägger till ett exempelvärde i cellen "A3"
worksheet.cells.get("A3").putValue(150);
//Lägger till ett diagram i kalkylbladet
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//Åtkomst till instansen av det nyss tillagda diagrammet
var chart = worksheet.charts.get(chartIndex);
//Lägger till NSeries (diagramdatakälla) till diagrammet från cell "A1" till "A3"
chart.nSeries.add("A1:A3", true);
chart.nSeries.get(0).area.invertIfNegative = true;
//Ställer in förgrundsfärgen för det första NSeries-området
chart.nSeries.get(0).area.foregroundColor = Color.Red;
//Ställer in bakgrundsfärgen för det första NSeries-området.
//Den visade områdesfärgen för den andra diagrampunkten blir bakgrundsfärgen.
chart.nSeries.get(0).area.backgroundColor = Color.Yellow;
//Sparar Excel-filen
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



