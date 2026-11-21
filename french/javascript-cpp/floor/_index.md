---
title: Floor
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates the object that represents the floor of a 3D chart.
type: docs
url: /fr/javascript-cpp/floor/
---

## Floor class

Encapsulates the object that represents the floor of a 3-D chart.

```javascript
class Floor extends Area;
```


### Example
```javascript
const { License, Workbook, ChartType, Color, GradientPresetType, GradientStyleType, SaveFormat } = AsposeCells;

//Instancier la classe License
var license = new License();
license.setLicense(data);

//Instancier l'objet classeur
var workbook = new Workbook();
//Obtenir la collection de cellules
var cells = workbook.worksheets.get(0).cells;
//Mettre des valeurs dans les cellules
cells.get("A1").putValue(1);
cells.get("A2").putValue(2);
cells.get("A3").putValue(3);

//obtenir la collection de graphiques
var charts = workbook.worksheets.get(0).charts;
//ajouter un nouveau graphique 
var index = charts.add(ChartType.Column3DStacked, 5, 0, 15, 5);
//obtenir le graphique récemment ajouté
var chart = charts.get(index);
//définir les séries du graphique
chart.nSeries.add("A1:A3", true);
//Afficher les étiquettes de données
chart.nSeries.get(0).dataLabels.showValue = true;

//Obtenir le plan du graphique
var floor = chart.floor;
//définir la bordure du plan en rouge
floor.border.color = new Color("red");
//définir le format de remplissage
floor.fillFormat.setPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.DiagonalDown, 2);

//enregistrer le fichier
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



