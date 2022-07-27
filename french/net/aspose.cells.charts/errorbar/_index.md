---
title: ErrorBar
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente la barre derreur de la série de données.
type: docs
weight: 630
url: /fr/net/aspose.cells.charts/errorbar/
---
## ErrorBar class

Représente la barre d'erreur de la série de données.

```csharp
public class ErrorBar : Line
```

## Propriétés

| Nom | La description |
| --- | --- |
| [Amount](../../aspose.cells.charts/errorbar/amount) { get; set; } | Représente la quantité de barre d'erreur.  Le montant doit être supérieur ou égal à zéro. |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength) { get; set; } | Spécifie la longueur de la pointe de flèche pour le début d'une ligne. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth) { get; set; } | Spécifie la largeur de la pointe de flèche pour le début d'une ligne. |
| [BeginType](../../aspose.cells.drawing/line/begintype) { get; set; } | Spécifie une pointe de flèche pour le début d'une ligne. |
| [CapType](../../aspose.cells.drawing/line/captype) { get; set; } | Spécifie les majuscules de fin. |
| [Color](../../aspose.cells.drawing/line/color) { get; set; } | Représente leColor de la ligne. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype) { get; set; } | Spécifie le type de ligne composée |
| [DashType](../../aspose.cells.drawing/line/dashtype) { get; set; } | Spécifie le type de ligne en tirets |
| [DisplayType](../../aspose.cells.charts/errorbar/displaytype) { get; set; } | Représente le type d'affichage de la barre d'erreur. |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength) { get; set; } | Spécifie la longueur de la pointe de flèche pour la fin d'une ligne. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth) { get; set; } | Spécifie la largeur de la pointe de flèche pour la fin d'une ligne. |
| [EndType](../../aspose.cells.drawing/line/endtype) { get; set; } | Spécifie une pointe de flèche pour la fin d'une ligne. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype) { get; set; } | Obtient ou définit le type de format. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill) { get; } | Représente le remplissage dégradé. |
| [IsAuto](../../aspose.cells.drawing/line/isauto) { get; set; } | Indique si ce style de trait est attribué automatiquement. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor) { get; } | Indique si la couleur de la ligne est attribuée automatiquement. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible) { get; set; } | Indique si la ligne est visible. |
| [JoinType](../../aspose.cells.drawing/line/jointype) { get; set; } | Spécifie les majuscules de jonction. |
| [MinusValue](../../aspose.cells.charts/errorbar/minusvalue) { get; set; } | Représente le montant d'erreur négatif lorsque le type de barre d'erreur est Personnalisé. |
| [PlusValue](../../aspose.cells.charts/errorbar/plusvalue) { get; set; } | Représente le montant d'erreur positif lorsque le type de barre d'erreur est Personnalisé. |
| [ShowMarkerTTop](../../aspose.cells.charts/errorbar/showmarkerttop) { get; set; } | Indique si le formatage des barres d'erreur avec un T-top. |
| [Style](../../aspose.cells.drawing/line/style) { get; set; } | Représente le style de la ligne. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor) { get; set; } | Obtient et définit la couleur du thème. |
| [Transparency](../../aspose.cells.drawing/line/transparency) { get; set; } | Renvoie ou définit le degré de transparence de la ligne sous la forme d'une valeur comprise entre 0,0 (opaque) et 1,0 (clair). |
| [Type](../../aspose.cells.charts/errorbar/type) { get; set; } | Représente le type de montant de la barre d'erreur. |
| [Weight](../../aspose.cells.drawing/line/weight) { get; set; } | Obtient ou définit le[`WeightType`](../../aspose.cells.drawing/weighttype) de la ligne. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt) { get; set; } | Obtient ou définit le poids de la ligne en unités de points. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx) { get; set; } | Obtient ou définit l'épaisseur de la ligne en pixels. |

### Exemples

```csharp
[C#]
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
cells["a1"].PutValue(2);
cells["a2"].PutValue(5);
cells["a3"].PutValue(3);
cells["a4"].PutValue(6);
cells["b1"].PutValue(4);
cells["b2"].PutValue(3);
cells["b3"].PutValue(6);
cells["b4"].PutValue(7);

cells["C1"].PutValue("Q1");
cells["C2"].PutValue("Q2");
cells["C3"].PutValue("Y1");
cells["C4"].PutValue("Y2");

int chartIndex = excel.Worksheets[0].Charts.Add(ChartType.Column, 11, 0, 27, 10);

Chart chart = excel.Worksheets[0].Charts[chartIndex];
chart.NSeries.Add("A1:B4", true);

chart.NSeries.CategoryData = "C1:C4";

for(int i = 0; i < chart.NSeries.Count; i ++)
{
	ASeries aseries = chart.NSeries[i];
	aseries.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
	aseries.YErrorBar.Type = ErrorBarType.FixedValue;
	aseries.YErrorBar.Amount = 5;
}

[Visual Basic]
Dim workbook As Workbook =  New Workbook() 
Dim cells As Cells =  workbook.Worksheets(0).Cells 
cells("a1").PutValue(2)
cells("a2").PutValue(5)
cells("a3").PutValue(3)
cells("a4").PutValue(6)
cells("b1").PutValue(4)
cells("b2").PutValue(3)
cells("b3").PutValue(6)
cells("b4").PutValue(7)

cells("C1").PutValue("Q1")
cells("C2").PutValue("Q2")
cells("C3").PutValue("Y1")
cells("C4").PutValue("Y2")

Dim chartIndex As Integer =  excel.Worksheets(0).Charts.Add(ChartType.Column,11,0,27,10) 

Dim chart As Chart =  excel.Worksheets(0).Charts(chartIndex) 
chart.NSeries.Add("A1:B4", True)

chart.NSeries.CategoryData = "C1:C4"

Dim i As Integer
For  i = 0 To chart.NSeries.Count - 1
Dim aseries As ASeries =  chart.NSeries(i) 
aseries.YErrorBar.DisplayType = ErrorBarDisplayType.Minus
aseries.YErrorBar.Type = ErrorBarType.FixedValue
aseries.YErrorBar.Amount = 5
Next
```

### Voir également

* class [Line](../../aspose.cells.drawing/line)
* espace de noms [Aspose.Cells.Charts](../../aspose.cells.charts)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
