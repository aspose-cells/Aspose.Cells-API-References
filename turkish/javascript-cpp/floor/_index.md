---
title: Floor
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates the object that represents the floor of a 3D chart.
type: docs
url: /tr/javascript-cpp/floor/
---

## Floor class

Encapsulates the object that represents the floor of a 3-D chart.

```javascript
class Floor extends Area;
```


### Example
```javascript
const { License, Workbook, ChartType, Color, GradientPresetType, GradientStyleType, SaveFormat } = AsposeCells;

//License sınıfını örnekle
var license = new License();
license.setLicense(data);

//Çalışma kitabı nesnesini örnekle
var workbook = new Workbook();
//Hücre koleksiyonunu al
var cells = workbook.worksheets.get(0).cells;
//Hücrelere değer koy
cells.get("A1").putValue(1);
cells.get("A2").putValue(2);
cells.get("A3").putValue(3);

//grafik koleksiyonunu al
var charts = workbook.worksheets.get(0).charts;
//yeni bir grafik ekle
var index = charts.add(ChartType.Column3DStacked, 5, 0, 15, 5);
//yeni eklenen grafiği al
var chart = charts.get(index);
//grafik nSeries'ı ayarla
chart.nSeries.add("A1:A3", true);
//Veri etiketlerini göster
chart.nSeries.get(0).dataLabels.showValue = true;

//Grafiğin zemini al
var floor = chart.floor;
//zeminin kenarlığını kırmızı olarak ayarla
floor.border.color = new Color("red");
//dolgu biçimini ayarla
floor.fillFormat.setPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.DiagonalDown, 2);

//dosyayı kaydet
var uint8Array = workbook.save(SaveFormat.Excel97To2003);
```
## Constructors

| Name | Description |
| --- | --- |
| [constructor(Area)](#constructor-area-)| Constructs from a parent object convertible to this. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [border](#border--)| Line | Gets or sets the border [Line](../line/). |
| [backgroundColor](#backgroundColor--)| Color | Gets or sets the background [Color](../color/) of the [Area](../area/). |
| [foregroundColor](#foregroundColor--)| Color | Gets or sets the foreground [Color](../color/). |
| [formatting](#formatting--)| FormattingType | Represents the formatting of the area. |
| [invertIfNegative](#invertIfNegative--)| boolean | If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [fillFormat](#fillFormat--)| FillFormat | Readonly. Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape. |
| [transparency](#transparency--)| number | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |


### constructor(Area) {#constructor-area-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: Area);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Area | The parent object. |

### border {#border--}

Gets or sets the border [Line](../line/).

```javascript
border : Line;
```


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



