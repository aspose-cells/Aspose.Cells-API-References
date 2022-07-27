---
title: Trendline
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente une ligne de tendance dans un graphique.
type: docs
weight: 980
url: /fr/net/aspose.cells.charts/trendline/
---
## Trendline class

Représente une ligne de tendance dans un graphique.

```csharp
public class Trendline : Line
```

## Propriétés

| Nom | La description |
| --- | --- |
| [Backward](../../aspose.cells.charts/trendline/backward) { get; set; } | Renvoie ou définit le nombre de périodes (ou d'unités sur un graphique en nuage de points) pendant lesquelles la ligne de tendance s'étend vers l'arrière. Le nombre de périodes doit être supérieur ou égal à zéro. Si le type de graphique est colonne, le nombre de périodes doit être compris entre 0 et 0,5 |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength) { get; set; } | Spécifie la longueur de la pointe de flèche pour le début d'une ligne. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth) { get; set; } | Spécifie la largeur de la pointe de flèche pour le début d'une ligne. |
| [BeginType](../../aspose.cells.drawing/line/begintype) { get; set; } | Spécifie une pointe de flèche pour le début d'une ligne. |
| [CapType](../../aspose.cells.drawing/line/captype) { get; set; } | Spécifie les majuscules de fin. |
| [Color](../../aspose.cells.drawing/line/color) { get; set; } | Représente leColor de la ligne. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype) { get; set; } | Spécifie le type de ligne composée |
| [DashType](../../aspose.cells.drawing/line/dashtype) { get; set; } | Spécifie le type de ligne en tirets |
| [DataLabels](../../aspose.cells.charts/trendline/datalabels) { get; } | Représente l'objet DataLabels pour la série spécifiée. |
| [DisplayEquation](../../aspose.cells.charts/trendline/displayequation) { get; set; } | Représente si l'équation de la ligne de tendance est affichée sur le graphique (dans la même étiquette de données que la valeur R au carré). La définition de cette propriété sur True active automatiquement les étiquettes de données. |
| [DisplayRSquared](../../aspose.cells.charts/trendline/displayrsquared) { get; set; } | Représente si la valeur R au carré de la courbe de tendance est affichée sur le graphique (dans la même étiquette de données que l'équation). La définition de cette propriété sur True active automatiquement les étiquettes de données. |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength) { get; set; } | Spécifie la longueur de la pointe de flèche pour la fin d'une ligne. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth) { get; set; } | Spécifie la largeur de la pointe de flèche pour la fin d'une ligne. |
| [EndType](../../aspose.cells.drawing/line/endtype) { get; set; } | Spécifie une pointe de flèche pour la fin d'une ligne. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype) { get; set; } | Obtient ou définit le type de format. |
| [Forward](../../aspose.cells.charts/trendline/forward) { get; set; } | Renvoie ou définit le nombre de périodes (ou d'unités sur un graphique en nuage de points) que la ligne de tendance étend vers l'avant. Le nombre de périodes doit être supérieur ou égal à zéro. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill) { get; } | Représente le remplissage dégradé. |
| [Intercept](../../aspose.cells.charts/trendline/intercept) { get; set; } | Renvoie ou définit le point où la courbe de tendance croise l'axe des valeurs. |
| [IsAuto](../../aspose.cells.drawing/line/isauto) { get; set; } | Indique si ce style de trait est attribué automatiquement. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor) { get; } | Indique si la couleur de la ligne est attribuée automatiquement. |
| [IsNameAuto](../../aspose.cells.charts/trendline/isnameauto) { get; set; } | Renvoie si Microsoft Excel détermine automatiquement le nom de la courbe de tendance. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible) { get; set; } | Indique si la ligne est visible. |
| [JoinType](../../aspose.cells.drawing/line/jointype) { get; set; } | Spécifie les majuscules de jonction. |
| [LegendEntry](../../aspose.cells.charts/trendline/legendentry) { get; } | Obtient l'entrée de légende selon cette ligne de tendance |
| [Name](../../aspose.cells.charts/trendline/name) { get; set; } | Renvoie le nom de la ligne de tendance. |
| [Order](../../aspose.cells.charts/trendline/order) { get; set; } | Renvoie ou définit l'ordre de la ligne de tendance (un entier supérieur à 1) lorsque le type de ligne de tendance est polynomial. La commande doit être comprise entre 2 et 6. |
| [Period](../../aspose.cells.charts/trendline/period) { get; set; } | Renvoie ou définit la période de la ligne de tendance moyenne mobile. |
| [Style](../../aspose.cells.drawing/line/style) { get; set; } | Représente le style de la ligne. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor) { get; set; } | Obtient et définit la couleur du thème. |
| [Transparency](../../aspose.cells.drawing/line/transparency) { get; set; } | Renvoie ou définit le degré de transparence de la ligne sous la forme d'une valeur comprise entre 0,0 (opaque) et 1,0 (clair). |
| [Type](../../aspose.cells.charts/trendline/type) { get; } | Renvoie le type de ligne de tendance. |
| [Weight](../../aspose.cells.drawing/line/weight) { get; set; } | Obtient ou définit le[`WeightType`](../../aspose.cells.drawing/weighttype) de la ligne. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt) { get; set; } | Obtient ou définit le poids de la ligne en unités de points. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx) { get; set; } | Obtient ou définit l'épaisseur de la ligne en pixels. |

### Exemples

```csharp

[C#]

//Instanciation d'un objet Workbook
Workbook workbook = new Workbook();
//Ajout d'une nouvelle feuille de calcul à l'objet Excel
int sheetIndex = workbook.Worksheets.Add();
//Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son index de feuille
Worksheet worksheet = workbook.Worksheets[sheetIndex];
//Ajout d'un exemple de valeur à la cellule "A1"
worksheet.Cells["A1"].PutValue(50);
//Ajout d'un exemple de valeur à la cellule "A2"
worksheet.Cells["A2"].PutValue(100);
//Ajout d'un exemple de valeur à la cellule "A3"
worksheet.Cells["A3"].PutValue(150);
//Ajout d'un exemple de valeur à la cellule "A4"
worksheet.Cells["A4"].PutValue(200);
//Ajout d'un exemple de valeur à la cellule "B1"
worksheet.Cells["B1"].PutValue(60);
//Ajout d'un exemple de valeur à la cellule "B2"
worksheet.Cells["B2"].PutValue(32);
//Ajout d'un exemple de valeur à la cellule "B3"
worksheet.Cells["B3"].PutValue(50);
//Ajout d'un exemple de valeur à la cellule "B4"
worksheet.Cells["B4"].PutValue(40);
//Ajout d'un exemple de valeur à la cellule "C1" en tant que données de catégorie
worksheet.Cells["C1"].PutValue("Q1");
//Ajout d'un exemple de valeur à la cellule "C2" en tant que données de catégorie
worksheet.Cells["C2"].PutValue("Q2");
//Ajout d'un exemple de valeur à la cellule "C3" en tant que données de catégorie
worksheet.Cells["C3"].PutValue("Y1");
//Ajout d'un exemple de valeur à la cellule "C4" en tant que données de catégorie
worksheet.Cells["C4"].PutValue("Y2");
//Ajout d'un graphique à la feuille de calcul
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
//Accéder à l'instance du graphique nouvellement ajouté
Chart chart = worksheet.Charts[chartIndex];
//Ajout de NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "B4"
chart.NSeries.Add("A1:B4", true);
//Définition de la source de données pour les données de catégorie de NSeries
chart.NSeries.CategoryData = "C1:C4";
//ajout d'une ligne de tendance linéaire
int index = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
Trendline trendline = chart.NSeries[0].TrendLines[index];
//Définition du nom personnalisé de la courbe de tendance.
trendline.Name = "Linear";
//Affichage de l'équation sur le graphique
trendline.DisplayEquation = true;
// Affichage de la valeur R-Squared sur le graphique
trendline.DisplayRSquared = true;
//Enregistrement du fichier Excel
workbook.Save("book1.xls");

[Visual Basic]

'Instanciation d'un objet Workbook
Dim workbook As Workbook = New Workbook()
'Ajout d'une nouvelle feuille de calcul à l'objet Excel
Dim sheetIndex As Int32 = workbook.Worksheets.Add()
'Obtenir la référence de la feuille de calcul nouvellement ajoutée en passant son index de feuille
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)
'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)
'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)
'Adding a sample value to "A4" cell
worksheet.Cells("A4").PutValue(200)
'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)
'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)
'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)
'Adding a sample value to "B4" cell
worksheet.Cells("B4").PutValue(40)
'Adding a sample value to "C1" cell as category data
worksheet.Cells("C1").PutValue("Q1")
'Adding a sample value to "C2" cell as category data
worksheet.Cells("C2").PutValue("Q2")
'Adding a sample value to "C3" cell as category data
worksheet.Cells("C3").PutValue("Y1")
'Adding a sample value to "C4" cell as category data
worksheet.Cells("C4").PutValue("Y2")
'Ajouter un graphique à la feuille de calcul
Dim chartIndex As Int32 = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Accéder à l'instance du graphique nouvellement ajouté
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.NSeries.Add("A1:B4", True)
'Définition de la source de données pour les données de catégorie de NSeries
Chart.NSeries.CategoryData = "C1:C4"
'ajouter une ligne de tendance linéaire
Dim index As Int32 = chart.NSeries(0).TrendLines.Add(TrendlineType.Linear)
Dim trendline As Trendline = chart.NSeries(0).TrendLines(index)
'Définition du nom personnalisé de la courbe de tendance.
trendline.Name = "Linear"
'Affichage de l'équation sur le graphique
trendline.DisplayEquation = True
'Affichage de la valeur R-Squared sur le graphique
trendline.DisplayRSquared = True
'Enregistrement du fichier Excel
workbook.Save("book1.xls")
```

### Voir également

* class [Line](../../aspose.cells.drawing/line)
* espace de noms [Aspose.Cells.Charts](../../aspose.cells.charts)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
