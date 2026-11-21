---
title: Area
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates the object that represents an area format.
type: docs
url: /es/javascript-cpp/area/
---

## Area class

Encapsulates the object that represents an area format.

```javascript
class Area;
```


### Example
```javascript
const { Workbook, ChartType, Color, SaveFormat } = AsposeCells;

//Instanciando un objeto Workbook
var workbook = new Workbook();
//Agregando una nueva hoja de trabajo al objeto Workbook
var sheetIndex = workbook.worksheets.add();
//Obteniendo la referencia de la hoja de cálculo recién añadida pasando su índice de hoja
var worksheet = workbook.worksheets.get(sheetIndex);
//Añadiendo un valor de muestra a la celda "A1"
worksheet.cells.get("A1").putValue(50);
//Añadiendo un valor de muestra a la celda "A2"
worksheet.cells.get("A2").putValue(100);
//Añadiendo un valor de muestra a la celda "A3"
worksheet.cells.get("A3").putValue(150);
//Añadiendo un valor de muestra a la celda "B1"
worksheet.cells.get("B1").putValue(60);
//Añadiendo un valor de muestra a la celda "B2"
worksheet.cells.get("B2").putValue(32);
//Añadiendo un valor de muestra a la celda "B3"
worksheet.cells.get("B3").putValue(50);
//Agregar un gráfico a la hoja de cálculo
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//Accediendo a la instancia del gráfico recién añadido
var chart = worksheet.charts.get(chartIndex);
//Agregar NSeries (fuente de datos del gráfico) al gráfico que abarca desde la celda "A1" hasta "B3"
chart.nSeries.add("A1:B3", true);
//Estableciendo el color de primer plano del área del gráfico
chart.plotArea.getArea().foregroundColor = Color.Blue;
//Estableciendo el color de primer plano del área del diagrama
chart.chartArea.getArea().foregroundColor = Color.Yellow;
//Estableciendo el color de primer plano del área de la 1ª NSeries
chart.nSeries.get(0).area.foregroundColor = Color.Red;
//Estableciendo el color de primer plano del área del punto de la 1ª NSeries
chart.nSeries.get(0).points.get(0).area.foregroundColor = Color.Cyan;
//Guardando el archivo Excel
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

//Instanciando un objeto Workbook
var workbook = new Workbook();
//Agregando una nueva hoja de trabajo al objeto Workbook
var sheetIndex = workbook.worksheets.add();
//Obteniendo la referencia de la hoja de cálculo recién añadida pasando su índice de hoja
var worksheet = workbook.worksheets.get(sheetIndex);
//Añadiendo un valor de muestra a la celda "A1"
worksheet.cells.get("A1").putValue(50);
//Añadiendo un valor de muestra a la celda "A2"
worksheet.cells.get("A2").putValue(-100);
//Añadiendo un valor de muestra a la celda "A3"
worksheet.cells.get("A3").putValue(150);
//Agregar un gráfico a la hoja de cálculo
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//Accediendo a la instancia del gráfico recién añadido
var chart = worksheet.charts.get(chartIndex);
//Agregando NSeries (fuente de datos del gráfico) al gráfico que abarca desde la celda "A1" hasta "A3"
chart.nSeries.add("A1:A3", true);
chart.nSeries.get(0).area.invertIfNegative = true;
//Estableciendo el color de primer plano del área de la 1ª NSeries
chart.nSeries.get(0).area.foregroundColor = Color.Red;
//Estableciendo el color de fondo del área de la 1ª NSeries.
//El color del área mostrada del segundo punto del gráfico será el color de fondo.
chart.nSeries.get(0).area.backgroundColor = Color.Yellow;
//Guardando el archivo Excel
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



