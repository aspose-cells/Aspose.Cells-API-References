---
title: DisplayUnitLabel
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente létiquette de lunité daffichage.
type: docs
weight: 600
url: /fr/net/aspose.cells.charts/displayunitlabel/
---
## DisplayUnitLabel class

Représente l'étiquette de l'unité d'affichage.

```csharp
public class DisplayUnitLabel : ChartTextFrame
```

## Propriétés

| Nom | La description |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | Obtient le[`Région`](../chartframe/area) . |
| override [AutoScaleFont](../../aspose.cells.charts/displayunitlabel/autoscalefont) { get; set; } | True si le texte de l'objet change de taille de police lorsque la taille de l'objet change. La valeur par défaut est Vrai. |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | Obtient et définit le mode d'affichage de l'arrière-plan |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | Obtient le[`frontière`](../../aspose.cells.drawing/line) . |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | Représente la hauteur de la position par défaut |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | Représente la largeur de la position par défaut |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | Représente x de la position par défaut |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | Représente y de la position par défaut |
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype) { get; set; } | Obtient et définit la direction du texte. |
| override [Font](../../aspose.cells.charts/displayunitlabel/font) { get; } | Obtient un[`Font`](./font) objet de l'objet ChartFrame spécifié. |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | Obtient ou définit la hauteur du cadre en unités de 1/4000 de la zone du graphique. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Indique si le cadre du graphique est dimensionné automatiquement. |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext) { get; set; } | Indique que le texte est généré automatiquement. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Indique si la position par défaut (DefaultX, DefaultY, DefaultWidth et DefaultHeight) est définie. |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | Indique si ces étiquettes de données sont supprimées. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Indique si la taille de la zone de tracé comprend les graduations et les étiquettes d'axe. False spécifie que la taille doit déterminer la taille de la zone de tracé, les graduations et les étiquettes d'axe. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | Obtient ou définit si une forme doit être ajustée automatiquement pour contenir entièrement le texte qui y est décrit. L'ajustement automatique est lorsque le texte d'une forme est mis à l'échelle afin de contenir tout le texte à l'intérieur. |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped) { get; set; } | Obtient ou définit une valeur indiquant si le texte est encapsulé. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | Obtient et définit une référence à la feuille de calcul. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | Représente l'ordre de lecture du texte. |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | Représente l'angle de rotation du texte. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | Vrai si le cadre a une ombre. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Obtient le[`ShapeProperties`](../chartframe/shapeproperties) objet. |
| override [Text](../../aspose.cells.charts/displayunitlabel/text) { get; set; } | Obtient ou définit le texte de l'étiquette de l'unité d'affichage. |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment) { get; set; } | Obtient et définit l'alignement horizontal du texte. |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment) { get; set; } | Obtient ou définit l'alignement vertical du texte. |
| virtual [Width](../../aspose.cells.charts/chartframe/width) { get; set; } | Obtient ou définit la largeur du cadre en unités de 1/4000 de la zone de graphique. |
| virtual [X](../../aspose.cells.charts/chartframe/x) { get; set; } | Obtient ou définit la coordonnée x du coin supérieur gauche en unités de 1/4000 de la zone de graphique. |
| virtual [Y](../../aspose.cells.charts/chartframe/y) { get; set; } | Obtient ou définit la coordonnée y du coin supérieur gauche en unités de 1/4000 de la zone du graphique. |

## Méthodes

| Nom | La description |
| --- | --- |
| [Characters](../../aspose.cells.charts/charttextframe/characters)(int, int) | Renvoie un objet Characters qui représente une plage de caractères dans le texte. |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | Définir la position du cadre sur automatique |

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
//Définition de l'unité d'affichage de l'axe des valeurs (Y).
chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
DisplayUnitLabel displayUnitLabel = chart.ValueAxis.DisplayUnitLabel;
//Définition de l'étiquette de l'unité d'affichage personnalisée
displayUnitLabel.Text = "100";
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
'Réglage de l'unité d'affichage de l'axe des valeurs (Y).
chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds
Dim displayUnitLabel As DisplayUnitLabel = chart.ValueAxis.DisplayUnitLabel
'Réglage de l'étiquette de l'unité d'affichage personnalisée
displayUnitLabel.Text = "100"
'Enregistrement du fichier Excel
workbook.Save("book1.xls")
```

### Voir également

* class [ChartTextFrame](../charttextframe)
* espace de noms [Aspose.Cells.Charts](../../aspose.cells.charts)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
