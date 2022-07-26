---
title: ChartArea
second_title: Référence de l'API Aspose.Cells pour .NET
description: Encapsule lobjet qui représente la zone de graphique dans la feuille de calcul.
type: docs
weight: 440
url: /fr/net/aspose.cells.charts/chartarea/
---
## ChartArea class

Encapsule l'objet qui représente la zone de graphique dans la feuille de calcul.

```csharp
public class ChartArea : ChartFrame
```

## Propriétés

| Nom | La description |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | Obtient le[`Région`](../chartframe/area) . |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont) { get; set; } | True si le texte de l'objet change de taille de police lorsque la taille de l'objet change. La valeur par défaut est Vrai. |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | Obtient et définit le mode d'affichage de l'arrière-plan |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | Obtient le[`frontière`](../../aspose.cells.drawing/line) . |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | Représente la hauteur de la position par défaut |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | Représente la largeur de la position par défaut |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | Représente x de la position par défaut |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | Représente y de la position par défaut |
| override [Font](../../aspose.cells.charts/chartarea/font) { get; } | Obtient un[`Font`](./font) objet de l'objet chartarea spécifié. |
| override [Height](../../aspose.cells.charts/chartarea/height) { get; set; } | Obtient ou définit le décalage vertical à partir de sa ligne du coin inférieur droit. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Indique si le cadre du graphique est dimensionné automatiquement. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Indique si la position par défaut (DefaultX, DefaultY, DefaultWidth et DefaultHeight) est définie. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Indique si la taille de la zone de tracé comprend les graduations et les étiquettes d'axe. False spécifie que la taille doit déterminer la taille de la zone de tracé, les graduations et les étiquettes d'axe. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | Vrai si le cadre a une ombre. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Obtient le[`ShapeProperties`](../chartframe/shapeproperties) objet. |
| override [Width](../../aspose.cells.charts/chartarea/width) { get; set; } | Obtient ou définit le décalage horizontal à partir de sa colonne d'angle inférieur droit. |
| override [X](../../aspose.cells.charts/chartarea/x) { get; set; } | Obtient ou obtient le décalage horizontal de sa colonne d'angle supérieur gauche. |
| override [Y](../../aspose.cells.charts/chartarea/y) { get; set; } | Obtient ou obtient le décalage vertical à partir de sa ligne du coin supérieur gauche. |

## Méthodes

| Nom | La description |
| --- | --- |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | Définir la position du cadre sur automatique |

### Exemples

```csharp

[C#]

//Instanciation d'un objet Workbook
Workbook workbook = new Workbook();

//Obtention de la référence de la première feuille de travail
Worksheet worksheet = workbook.Worksheets[0];

//Ajout d'un exemple de valeur à la cellule "A1"
worksheet.Cells["A1"].PutValue(50);

//Ajout d'un exemple de valeur à la cellule "A2"
worksheet.Cells["A2"].PutValue(100);

//Ajout d'un exemple de valeur à la cellule "A3"
worksheet.Cells["A3"].PutValue(150);

//Ajout d'un exemple de valeur à la cellule "B1"
worksheet.Cells["B1"].PutValue(60);

//Ajout d'un exemple de valeur à la cellule "B2"
worksheet.Cells["B2"].PutValue(32);

//Ajout d'un exemple de valeur à la cellule "B3"
worksheet.Cells["B3"].PutValue(50);

//Ajout d'un graphique à la feuille de calcul
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);

//Accéder à l'instance du graphique nouvellement ajouté
Chart chart = worksheet.Charts[chartIndex];

//Ajout de NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "B3"
chart.NSeries.Add("A1:B3", true);

// Obtention de la zone de graphique
ChartArea chartArea = chart.ChartArea;

//Définition de la couleur de premier plan de la zone du graphique
chartArea.Area.ForegroundColor = Color.Yellow;

//Définition de l'ombre de la zone de graphique
chartArea.Shadow = true;

//Enregistrement du fichier Excel
workbook.Save("book1.xls");

[VB.NET]

'Instanciation d'un objet Workbook
Dim workbook As Workbook = New Workbook()

'Obtention de la référence de la première feuille de travail
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)

'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)

'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)

'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)

'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)

'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)

'Ajouter un graphique à la feuille de calcul
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)

'Accéder à l'instance du graphique nouvellement ajouté
Dim chart As Chart = worksheet.Charts(chartIndex)

'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", True)

'Obtenir la zone de graphique
Dim chartArea As ChartArea = chart.ChartArea

'Définition de la couleur de premier plan de la zone de graphique
chartArea.Area.ForegroundColor = Color.Yellow

'Définition de l'ombre de la zone de graphique
chartArea.Shadow = True

'Enregistrement du fichier Excel
workbook.Save("book1.xls")
```

### Voir également

* class [ChartFrame](../chartframe)
* espace de noms [Aspose.Cells.Charts](../../aspose.cells.charts)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
