---
title: Legend
second_title: Référence de l'API Aspose.Cells pour .NET
description: Encapsule lobjet qui représente la légende du graphique.
type: docs
weight: 690
url: /fr/net/aspose.cells.charts/legend/
---
## Legend class

Encapsule l'objet qui représente la légende du graphique.

```csharp
public class Legend : ChartTextFrame
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
| [IsOverLay](../../aspose.cells.charts/legend/isoverlay) { get; set; } | Obtient ou définit si d'autres éléments de graphique doivent être autorisés à chevaucher cet élément de graphique. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | Obtient ou définit si une forme doit être ajustée automatiquement pour contenir entièrement le texte qui y est décrit. L'ajustement automatique est lorsque le texte d'une forme est mis à l'échelle afin de contenir tout le texte à l'intérieur. |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped) { get; set; } | Obtient ou définit une valeur indiquant si le texte est encapsulé. |
| [LegendEntries](../../aspose.cells.charts/legend/legendentries) { get; } | Obtient une collection de tous les objets LegendEntry dans la légende de graphique spécifiée. La définition des entrées de légende du graphique en surface n'est pas prise en charge. Il renverra donc null si le type de graphique est de type graphique en surface. |
| [LegendEntriesLabels](../../aspose.cells.charts/legend/legendentrieslabels) { get; } | Obtient les étiquettes des entrées de légende après l'appel de la méthode Chart.Calculate(). |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | Obtient et définit une référence à la feuille de calcul. |
| [Position](../../aspose.cells.charts/legend/position) { get; set; } | Obtient ou définit le type de position de la légende. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | Représente l'ordre de lecture du texte. |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | Représente l'angle de rotation du texte. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | Vrai si le cadre a une ombre. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Obtient le[`ShapeProperties`](../chartframe/shapeproperties) objet. |
| virtual [Text](../../aspose.cells.charts/charttextframe/text) { get; set; } | Obtient ou définit le texte du titre d'un cadre. |
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
chart.SetChartDataRange("A1:B4", true);
//Définir la largeur et la hauteur de la légende
Legend legend = chart.Legend;

//La légende est à droite du graphique par défaut.
// Si la légende se trouve à gauche ou à droite du graphique, la définition de la propriété Legend.X ne prendra pas effet.
//Si la légende est en haut ou en bas du graphique, la définition de la propriété Legend.Y ne prendra pas effet.
legend.Y = 1500;
legend.Width = 50;
legend.Height = 50; 
//Définir la position de la légende
legend.Position = LegendPositionType.Left;

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
		
Dim chartIndex as Integer = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15)

Dim chart as Chart = sheet.Charts(chartIndex)
chart.SetChartDataRange("A1:B4", True);
 
'Set Legend's width and height
Dim legend as Legend = chart.Legend

'La légende est à droite du graphique par défaut.
'Si la légende se trouve à gauche ou à droite du graphique, la définition de la propriété Legend.X ne prendra pas effet.
'Si la légende se trouve en haut ou en bas du graphique, la définition de la propriété Legend.Y ne prendra pas effet.
legend.Y = 1500
legend.Width = 50
legend.Height = 50
'Set legend's position
legend.Position = LegendPositionType.Left
```

### Voir également

* class [ChartTextFrame](../charttextframe)
* espace de noms [Aspose.Cells.Charts](../../aspose.cells.charts)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
