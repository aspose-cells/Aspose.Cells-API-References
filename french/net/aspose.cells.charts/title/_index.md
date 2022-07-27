---
title: Title
second_title: Référence de l'API Aspose.Cells pour .NET
description: Encapsule lobjet qui représente le titre du graphique ou de laxe.
type: docs
weight: 970
url: /fr/net/aspose.cells.charts/title/
---
## Title class

Encapsule l'objet qui représente le titre du graphique ou de l'axe.

```csharp
public class Title : ChartTextFrame
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
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype) { get; set; } | Obtient et définit la direction du texte. |
| virtual [Font](../../aspose.cells.charts/chartframe/font) { get; } | Obtient un[`Font`](../chartframe/font) objet de l'objet ChartFrame spécifié. |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | Obtient ou définit la hauteur du cadre en unités de 1/4000 de la zone du graphique. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Indique si le cadre du graphique est dimensionné automatiquement. |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext) { get; set; } | Indique que le texte est généré automatiquement. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Indique si la position par défaut (DefaultX, DefaultY, DefaultWidth et DefaultHeight) est définie. |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | Indique si ces étiquettes de données sont supprimées. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Indique si la taille de la zone de tracé comprend les graduations et les étiquettes d'axe. False spécifie que la taille doit déterminer la taille de la zone de tracé, les graduations et les étiquettes d'axe. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | Obtient ou définit si une forme doit être ajustée automatiquement pour contenir entièrement le texte qui y est décrit. L'ajustement automatique est lorsque le texte d'une forme est mis à l'échelle afin de contenir tout le texte à l'intérieur. |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped) { get; set; } | Obtient ou définit une valeur indiquant si le texte est encapsulé. |
| [IsVisible](../../aspose.cells.charts/title/isvisible) { get; set; } | Indique si le titre est visible. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | Obtient et définit une référence à la feuille de calcul. |
| [OverLay](../../aspose.cells.charts/title/overlay) { get; set; } | Représente le titre centré en superposition sur le graphique sans redimensionner le graphique. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | Représente l'ordre de lecture du texte. |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | Représente l'angle de rotation du texte. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | Vrai si le cadre a une ombre. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Obtient le[`ShapeProperties`](../chartframe/shapeproperties) objet. |
| override [Text](../../aspose.cells.charts/title/text) { get; set; } | Obtient ou définit le texte de l'étiquette de l'unité d'affichage. |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment) { get; set; } | Obtient et définit l'alignement horizontal du texte. |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment) { get; set; } | Obtient ou définit l'alignement vertical du texte. |
| virtual [Width](../../aspose.cells.charts/chartframe/width) { get; set; } | Obtient ou définit la largeur du cadre en unités de 1/4000 de la zone de graphique. |
| override [X](../../aspose.cells.charts/title/x) { get; set; } | Obtient ou définit la coordonnée x du coin supérieur gauche en unités de 1/4000 de la zone de graphique. |
| override [Y](../../aspose.cells.charts/title/y) { get; set; } | Obtient ou définit la coordonnée y du coin supérieur gauche en unités de 1/4000 de la zone du graphique. |

## Méthodes

| Nom | La description |
| --- | --- |
| [Characters](../../aspose.cells.charts/title/characters#characters_1)() | Obtient la mise en forme de texte enrichi de ce titre. |
| [Characters](../../aspose.cells.charts/charttextframe/characters)(int, int) | Renvoie un objet Characters qui représente une plage de caractères dans le texte. |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | Définir la position du cadre sur automatique |

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
		
int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
Chart chart = sheet.Charts[chartIndex];

//Définition du titre d'un graphique
chart.Title.Text = "Title";
//Définition de la couleur de police du titre du graphique sur bleu
chart.Title.Font.Color = Color.Blue;
//Définition du titre de l'axe des catégories du graphique
chart.CategoryAxis.Title.Text = "Category";
//Définition du titre de l'axe des valeurs du graphique
chart.ValueAxis.Title.Text = "Value";

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

'Définir le titre d'un graphique
chart.Title.Text = "Title"
'Définition de la couleur de police du titre du graphique sur bleu
chart.Title.Font.Color = Color.Blue
'Définition du titre de l'axe des catégories du graphique
chart.CategoryAxis.Title.Text = "Category"
'Définition du titre de l'axe des valeurs du graphique
chart.ValueAxis.Title.Text = "Value"

```

### Voir également

* class [ChartTextFrame](../charttextframe)
* espace de noms [Aspose.Cells.Charts](../../aspose.cells.charts)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
