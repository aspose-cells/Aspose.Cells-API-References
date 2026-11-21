---
title: Area
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates the object that represents an area format.
type: docs
url: /de/javascript-cpp/area/
---

## Area class

Encapsulates the object that represents an area format.

```javascript
class Area;
```


### Example
```javascript
const { Workbook, ChartType, Color, SaveFormat } = AsposeCells;

//Instanziieren eines Workbook-Objekts
var workbook = new Workbook();
//Ein neues Arbeitsblatt zum Workbook-Objekt hinzufügen
var sheetIndex = workbook.worksheets.add();
//Abrufen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergabe seines Blattindexes
var worksheet = workbook.worksheets.get(sheetIndex);
//Hinzufügen eines Beispielwerts zur Zelle "A1"
worksheet.cells.get("A1").putValue(50);
//Hinzufügen eines Beispielwerts zur Zelle "A2"
worksheet.cells.get("A2").putValue(100);
//Hinzufügen eines Beispielwerts zur Zelle "A3"
worksheet.cells.get("A3").putValue(150);
//Hinzufügen eines Beispielwerts zur Zelle "B1"
worksheet.cells.get("B1").putValue(60);
//Hinzufügen eines Beispielwerts zur Zelle "B2"
worksheet.cells.get("B2").putValue(32);
//Hinzufügen eines Beispielwerts zur Zelle "B3"
worksheet.cells.get("B3").putValue(50);
//Ein Diagramm zum Arbeitsblatt hinzufügen
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//Zugriff auf die Instanz des neu hinzugefügten Diagramms
var chart = worksheet.charts.get(chartIndex);
//Hinzufügen von NSeries (Diagrammdatenquelle) zum Diagramm vom Feld "A1" bis "B3"
chart.nSeries.add("A1:B3", true);
//Festlegen der Vordergrundfarbe des Diagrammbereichs
chart.plotArea.getArea().foregroundColor = Color.Blue;
//Festlegen der Vordergrundfarbe des Chartbereichs
chart.chartArea.getArea().foregroundColor = Color.Yellow;
//Festlegen der Vordergrundfarbe des 1. NSeries-Bereichs
chart.nSeries.get(0).area.foregroundColor = Color.Red;
//Festlegen der Vordergrundfarbe des Bereichs des 1. NSeries-Punktes
chart.nSeries.get(0).points.get(0).area.foregroundColor = Color.Cyan;
//Speichern der Excel-Datei
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

//Instanziieren eines Workbook-Objekts
var workbook = new Workbook();
//Ein neues Arbeitsblatt zum Workbook-Objekt hinzufügen
var sheetIndex = workbook.worksheets.add();
//Abrufen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergabe seines Blattindexes
var worksheet = workbook.worksheets.get(sheetIndex);
//Hinzufügen eines Beispielwerts zur Zelle "A1"
worksheet.cells.get("A1").putValue(50);
//Hinzufügen eines Beispielwerts zur Zelle "A2"
worksheet.cells.get("A2").putValue(-100);
//Hinzufügen eines Beispielwerts zur Zelle "A3"
worksheet.cells.get("A3").putValue(150);
//Ein Diagramm zum Arbeitsblatt hinzufügen
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//Zugriff auf die Instanz des neu hinzugefügten Diagramms
var chart = worksheet.charts.get(chartIndex);
//Hinzufügen von NSeries (Diagrammdatenquelle) zum Diagramm von Zelle "A1" bis "A3"
chart.nSeries.add("A1:A3", true);
chart.nSeries.get(0).area.invertIfNegative = true;
//Festlegen der Vordergrundfarbe des 1. NSeries-Bereichs
chart.nSeries.get(0).area.foregroundColor = Color.Red;
//Festlegen der Hintergrundfarbe des 1. NSeries-Bereichs.
//Die angezeigte Flächenfarbe des zweiten Diagrammpunkts wird die Hintergrundfarbe sein.
chart.nSeries.get(0).area.backgroundColor = Color.Yellow;
//Speichern der Excel-Datei
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



