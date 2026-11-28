---
title: Area
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the object that represents an area format.
type: docs
url: /es/nodejs-cpp/area/
---

## Area class

Encapsulates the object that represents an area format.

```javascript
class Area;
```


### Example
```javascript
const { Workbook, ChartType, Color } = require("aspose.cells.node");

//Instanciando un objeto Workbook
var workbook = new Workbook();
//Agregando una nueva hoja de cálculo al objeto Workbook
var sheetIndex = workbook.worksheets.add();
//Obteniendo la referencia de la hoja de cálculo recién añadida pasando su índice de hoja
var worksheet = workbook.worksheets.get(sheetIndex);
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
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//Accediendo a la instancia del gráfico recién agregado
var chart = worksheet.charts.get(chartIndex);
//Agregar NSeries (fuente de datos del gráfico) al gráfico que abarca desde la celda "A1" hasta "B3"
chart.nSeries.add("A1:B3", true);
//Estableciendo el color de primer plano del área de trazado
chart.plotArea.getArea().foregroundColor = Color.Blue;
//Estableciendo el color de primer plano del área del gráfico
chart.chartArea.getArea().foregroundColor = Color.Yellow;
//Estableciendo el color de primer plano del área de la 1st NSeries
chart.nSeries.get(0).area.foregroundColor = Color.Red;
//Estableciendo el color de primer plano del área del punto de la 1st NSeries
chart.nSeries.get(0).points.get(0).area.foregroundColor = Color.Cyan;
//Guardando el archivo Excel
workbook.save("output/DrawingArea.xls");
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

## Methods

| Method | Description |
| --- | --- |
| [getBackgroundColor()](#getBackgroundColor--)| <b>@deprecated.</b> Please use the 'backgroundColor' property instead. Gets or sets the background [Color](../color/) of the [Area](../area/). |
| [setBackgroundColor(Color)](#setBackgroundColor-color-)| <b>@deprecated.</b> Please use the 'backgroundColor' property instead. Gets or sets the background [Color](../color/) of the [Area](../area/). |
| [getForegroundColor()](#getForegroundColor--)| <b>@deprecated.</b> Please use the 'foregroundColor' property instead. Gets or sets the foreground [Color](../color/). |
| [setForegroundColor(Color)](#setForegroundColor-color-)| <b>@deprecated.</b> Please use the 'foregroundColor' property instead. Gets or sets the foreground [Color](../color/). |
| [getFormatting()](#getFormatting--)| <b>@deprecated.</b> Please use the 'formatting' property instead. Represents the formatting of the area. |
| [setFormatting(FormattingType)](#setFormatting-formattingtype-)| <b>@deprecated.</b> Please use the 'formatting' property instead. Represents the formatting of the area. |
| [getInvertIfNegative()](#getInvertIfNegative--)| <b>@deprecated.</b> Please use the 'invertIfNegative' property instead. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [setInvertIfNegative(boolean)](#setInvertIfNegative-boolean-)| <b>@deprecated.</b> Please use the 'invertIfNegative' property instead. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [getFillFormat()](#getFillFormat--)| <b>@deprecated.</b> Please use the 'fillFormat' property instead. Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape. |
| [getTransparency()](#getTransparency--)| <b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTransparency(number)](#setTransparency-number-)| <b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


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
const { Workbook, ChartType, Color } = require("aspose.cells.node");

//Instanciando un objeto Workbook
var workbook = new Workbook();
//Agregando una nueva hoja de cálculo al objeto Workbook
var sheetIndex = workbook.worksheets.add();
//Obteniendo la referencia de la hoja de cálculo recién añadida pasando su índice de hoja
var worksheet = workbook.worksheets.get(sheetIndex);
//Añadiendo un valor de ejemplo a la celda "A1"
worksheet.cells.get("A1").putValue(50);
//Añadiendo un valor de ejemplo a la celda "A2"
worksheet.cells.get("A2").putValue(-100);
//Añadiendo un valor de ejemplo a la celda "A3"
worksheet.cells.get("A3").putValue(150);
//Agregar un gráfico a la hoja de cálculo
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//Accediendo a la instancia del gráfico recién agregado
var chart = worksheet.charts.get(chartIndex);
//Agregando NSeries (fuente de datos del gráfico) al gráfico que abarca desde la celda "A1" hasta "A3"
chart.nSeries.add("A1:A3", true);
chart.nSeries.get(0).area.invertIfNegative = true;
//Estableciendo el color de primer plano del área de la 1st NSeries
chart.nSeries.get(0).area.foregroundColor = Color.Red;
//Estableciendo el color de fondo del área de la 1st NSeries.
//El color del área mostrada del segundo punto del gráfico será el color de fondo.
chart.nSeries.get(0).area.backgroundColor = Color.Yellow;
//Guardando el archivo Excel
workbook.save("output/DrawingAreaInverseIfNegative.xls");
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


### getBackgroundColor() {#getBackgroundColor--}

<b>@deprecated.</b> Please use the 'backgroundColor' property instead. Gets or sets the background [Color](../color/) of the [Area](../area/).

```javascript
getBackgroundColor() : Color;
```


**Returns**

[Color](../color/)

### setBackgroundColor(Color) {#setBackgroundColor-color-}

<b>@deprecated.</b> Please use the 'backgroundColor' property instead. Gets or sets the background [Color](../color/) of the [Area](../area/).

```javascript
setBackgroundColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |

### getForegroundColor() {#getForegroundColor--}

<b>@deprecated.</b> Please use the 'foregroundColor' property instead. Gets or sets the foreground [Color](../color/).

```javascript
getForegroundColor() : Color;
```


**Returns**

[Color](../color/)

### setForegroundColor(Color) {#setForegroundColor-color-}

<b>@deprecated.</b> Please use the 'foregroundColor' property instead. Gets or sets the foreground [Color](../color/).

```javascript
setForegroundColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |

### getFormatting() {#getFormatting--}

<b>@deprecated.</b> Please use the 'formatting' property instead. Represents the formatting of the area.

```javascript
getFormatting() : FormattingType;
```


**Returns**

[FormattingType](../formattingtype/)

### setFormatting(FormattingType) {#setFormatting-formattingtype-}

<b>@deprecated.</b> Please use the 'formatting' property instead. Represents the formatting of the area.

```javascript
setFormatting(value: FormattingType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FormattingType](../formattingtype/) | The value to set. |

### getInvertIfNegative() {#getInvertIfNegative--}

<b>@deprecated.</b> Please use the 'invertIfNegative' property instead. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```javascript
getInvertIfNegative() : boolean;
```


### setInvertIfNegative(boolean) {#setInvertIfNegative-boolean-}

<b>@deprecated.</b> Please use the 'invertIfNegative' property instead. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```javascript
setInvertIfNegative(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getFillFormat() {#getFillFormat--}

<b>@deprecated.</b> Please use the 'fillFormat' property instead. Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape.

```javascript
getFillFormat() : FillFormat;
```


**Returns**

[FillFormat](../fillformat/)

### getTransparency() {#getTransparency--}

<b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

```javascript
getTransparency() : number;
```


### setTransparency(number) {#setTransparency-number-}

<b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

```javascript
setTransparency(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



