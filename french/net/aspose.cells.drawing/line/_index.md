---
title: Line
second_title: Référence de l'API Aspose.Cells pour .NET
description: Encapsule lobjet qui représente le format de ligne.
type: docs
weight: 2200
url: /fr/net/aspose.cells.drawing/line/
---
## Line class

Encapsule l'objet qui représente le format de ligne.

```csharp
public class Line
```

## Propriétés

| Nom | La description |
| --- | --- |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength) { get; set; } | Spécifie la longueur de la pointe de flèche pour le début d'une ligne. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth) { get; set; } | Spécifie la largeur de la pointe de flèche pour le début d'une ligne. |
| [BeginType](../../aspose.cells.drawing/line/begintype) { get; set; } | Spécifie une pointe de flèche pour le début d'une ligne. |
| [CapType](../../aspose.cells.drawing/line/captype) { get; set; } | Spécifie les majuscules de fin. |
| [Color](../../aspose.cells.drawing/line/color) { get; set; } | Représente leColor de la ligne. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype) { get; set; } | Spécifie le type de ligne composée |
| [DashType](../../aspose.cells.drawing/line/dashtype) { get; set; } | Spécifie le type de ligne en tirets |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength) { get; set; } | Spécifie la longueur de la pointe de flèche pour la fin d'une ligne. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth) { get; set; } | Spécifie la largeur de la pointe de flèche pour la fin d'une ligne. |
| [EndType](../../aspose.cells.drawing/line/endtype) { get; set; } | Spécifie une pointe de flèche pour la fin d'une ligne. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype) { get; set; } | Obtient ou définit le type de format. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill) { get; } | Représente le remplissage dégradé. |
| [IsAuto](../../aspose.cells.drawing/line/isauto) { get; set; } | Indique si ce style de trait est attribué automatiquement. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor) { get; } | Indique si la couleur de la ligne est attribuée automatiquement. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible) { get; set; } | Indique si la ligne est visible. |
| [JoinType](../../aspose.cells.drawing/line/jointype) { get; set; } | Spécifie les majuscules de jonction. |
| [Style](../../aspose.cells.drawing/line/style) { get; set; } | Représente le style de la ligne. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor) { get; set; } | Obtient et définit la couleur du thème. |
| [Transparency](../../aspose.cells.drawing/line/transparency) { get; set; } | Renvoie ou définit le degré de transparence de la ligne sous la forme d'une valeur comprise entre 0,0 (opaque) et 1,0 (clair). |
| [Weight](../../aspose.cells.drawing/line/weight) { get; set; } | Obtient ou définit le[`WeightType`](../weighttype) de la ligne. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt) { get; set; } | Obtient ou définit le poids de la ligne en unités de points. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx) { get; set; } | Obtient ou définit l'épaisseur de la ligne en pixels. |

### Exemples

```csharp

[C#]

Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];

Cells cells = sheet.Cells;
cells[0,1].PutValue("Income");
cells[1,0].PutValue("Company A");
cells[2,0].PutValue("Company B");
cells[3,0].PutValue("Company C");
cells[1,1].PutValue(10000);
cells[2,1].PutValue(20000);
cells[3,1].PutValue(30000);

int chartIndex = sheet.Charts.Add(ChartType.Line, 9, 9, 21, 15);
Chart chart = sheet.Charts[chartIndex];
//Appliquer un style pointillé sur les lignes d'un NSeries
chart.NSeries[0].Border.Style = LineType.Dot;
chart.NSeries[0].Border.Color = Color.Red;
//Appliquer un style de marqueur triangulaire sur les marqueurs de données d'un NSeries
chart.NSeries[0].Marker.MarkerStyle = ChartMarkerType.Triangle;
//Réglage du poids de toutes les lignes d'un NSeries sur moyen
chart.NSeries[0].Border.Weight = WeightType.MediumLine;

[Visual Basic]

Dim workbook as Workbook = new Workbook()
Dim sheet as Worksheet = workbook.Worksheets(0)

Dim cells as Cells = sheet.Cells
cells(0,1).PutValue("Income")
cells(1,0).PutValue("Company A")
cells(2,0).PutValue("Company B")
cells(3,0).PutValue("Company C")
cells(1,1).PutValue(10000)
cells(2,1).PutValue(20000)
cells(3,1).PutValue(30000)
		
Dim chartIndex as Integer = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15)    ///
Dim chart as Chart = sheet.Charts(chartIndex)
'Appliquer un style de ligne pointillée sur les lignes d'un NSeries
chart.NSeries(0).Border.Style = LineType.Dot
chart.NSeries(0).Border.Color = Color.Red
'Application d'un style de marqueur triangulaire sur les marqueurs de données d'un NSeries
chart.NSeries(0).Marker.MarkerStyle = ChartMarkerType.Triangle
'Définition de l'épaisseur de toutes les lignes d'un NSeries sur moyen
chart.NSeries(0).Border.Weight = WeightType.MediumLine
```

### Voir également

* espace de noms [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
