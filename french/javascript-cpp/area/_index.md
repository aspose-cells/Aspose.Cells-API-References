---
title: Area
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates the object that represents an area format.
type: docs
url: /fr/javascript-cpp/area/
---

## Area class

Encapsulates the object that represents an area format.

```javascript
class Area;
```


### Example
```javascript
const { Workbook, ChartType, Color, SaveFormat } = AsposeCells;

//Instanciation d'un objet Workbook
var workbook = new Workbook();
//Ajout d'une nouvelle feuille de calcul à l'objet Workbook
var sheetIndex = workbook.worksheets.add();
//Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son indice de feuille
var worksheet = workbook.worksheets.get(sheetIndex);
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
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//Accès à l'instance du graphique nouvellement ajouté
var chart = worksheet.charts.get(chartIndex);
//Ajouter NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "B3"
chart.nSeries.add("A1:B3", true);
//Définir la couleur de premier plan de la zone de tracé
chart.plotArea.getArea().foregroundColor = Color.Blue;
//Définir la couleur de premier plan de la zone du graphique
chart.chartArea.getArea().foregroundColor = Color.Yellow;
//Définir la couleur de premier plan de la zone du 1er NSeries
chart.nSeries.get(0).area.foregroundColor = Color.Red;
//Définir la couleur de premier plan de la zone du 1er point NSeries
chart.nSeries.get(0).points.get(0).area.foregroundColor = Color.Cyan;
//Enregistrement du fichier Excel
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

//Instanciation d'un objet Workbook
var workbook = new Workbook();
//Ajout d'une nouvelle feuille de calcul à l'objet Workbook
var sheetIndex = workbook.worksheets.add();
//Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son indice de feuille
var worksheet = workbook.worksheets.get(sheetIndex);
//Ajout d'une valeur d'exemple à la cellule "A1"
worksheet.cells.get("A1").putValue(50);
//Ajout d'une valeur d'exemple à la cellule "A2"
worksheet.cells.get("A2").putValue(-100);
//Ajout d'une valeur d'exemple à la cellule "A3"
worksheet.cells.get("A3").putValue(150);
//Ajout d'un graphique à la feuille de calcul
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//Accès à l'instance du graphique nouvellement ajouté
var chart = worksheet.charts.get(chartIndex);
//Ajout de NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "A3"
chart.nSeries.add("A1:A3", true);
chart.nSeries.get(0).area.invertIfNegative = true;
//Définir la couleur de premier plan de la zone du 1er NSeries
chart.nSeries.get(0).area.foregroundColor = Color.Red;
//Définir la couleur d'arrière-plan de la zone du 1er NSeries.
//La couleur de zone affichée du deuxième point du graphique sera la couleur d'arrière-plan.
chart.nSeries.get(0).area.backgroundColor = Color.Yellow;
//Enregistrement du fichier Excel
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



