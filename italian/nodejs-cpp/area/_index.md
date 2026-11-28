---
title: Area
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the object that represents an area format.
type: docs
url: /it/nodejs-cpp/area/
---

## Area class

Encapsulates the object that represents an area format.

```javascript
class Area;
```


### Example
```javascript
const { Workbook, ChartType, Color } = require("aspose.cells.node");

//Istanziare un oggetto Workbook
var workbook = new Workbook();
//Aggiunta di un nuovo foglio di lavoro all'oggetto Workbook
var sheetIndex = workbook.worksheets.add();
//Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice di foglio
var worksheet = workbook.worksheets.get(sheetIndex);
//Aggiungere un valore di esempio alla cella "A1"
worksheet.cells.get("A1").putValue(50);
//Aggiungere un valore di esempio alla cella "A2"
worksheet.cells.get("A2").putValue(100);
//Aggiungere un valore di esempio alla cella "A3"
worksheet.cells.get("A3").putValue(150);
//Aggiungere un valore di esempio alla cella "B1"
worksheet.cells.get("B1").putValue(60);
//Aggiungere un valore di esempio alla cella "B2"
worksheet.cells.get("B2").putValue(32);
//Aggiungere un valore di esempio alla cella "B3"
worksheet.cells.get("B3").putValue(50);
//Aggiunta di un grafico al foglio di lavoro
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//Accesso all'istanza del grafico appena aggiunto
var chart = worksheet.charts.get(chartIndex);
//Aggiunta di NSeries (origine dati del grafico) al grafico dall'intervallo di celle "A1" a "B3"
chart.nSeries.add("A1:B3", true);
//Impostare il colore di primo piano dell'area del grafico
chart.plotArea.getArea().foregroundColor = Color.Blue;
//Impostare il colore di primo piano dell'area del diagramma
chart.chartArea.getArea().foregroundColor = Color.Yellow;
//Impostare il colore di primo piano dell'area della prima NSeries
chart.nSeries.get(0).area.foregroundColor = Color.Red;
//Impostare il colore di primo piano dell'area del primo punto NSeries
chart.nSeries.get(0).points.get(0).area.foregroundColor = Color.Cyan;
//Salvare il file Excel
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

//Istanziare un oggetto Workbook
var workbook = new Workbook();
//Aggiunta di un nuovo foglio di lavoro all'oggetto Workbook
var sheetIndex = workbook.worksheets.add();
//Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice di foglio
var worksheet = workbook.worksheets.get(sheetIndex);
//Aggiungere un valore di esempio alla cella "A1"
worksheet.cells.get("A1").putValue(50);
//Aggiungere un valore di esempio alla cella "A2"
worksheet.cells.get("A2").putValue(-100);
//Aggiungere un valore di esempio alla cella "A3"
worksheet.cells.get("A3").putValue(150);
//Aggiunta di un grafico al foglio di lavoro
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//Accesso all'istanza del grafico appena aggiunto
var chart = worksheet.charts.get(chartIndex);
//Aggiungere NSeries (fonte dati del diagramma) al diagramma dall'intervallo della cella "A1" alla cella "A3"
chart.nSeries.add("A1:A3", true);
chart.nSeries.get(0).area.invertIfNegative = true;
//Impostare il colore di primo piano dell'area della prima NSeries
chart.nSeries.get(0).area.foregroundColor = Color.Red;
//Impostare il colore di sfondo dell'area della prima NSeries.
//Il colore dell'area visualizzata del secondo punto del diagramma sarà il colore di sfondo.
chart.nSeries.get(0).area.backgroundColor = Color.Yellow;
//Salvare il file Excel
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



