---
title: DataLabels
second_title: Référence de l'API Aspose.Cells pour .NET
description: Encapsule une collection de tous les objets DataLabel pour la série spécifiée.
type: docs
weight: 580
url: /fr/net/aspose.cells.charts/datalabels/
---
## DataLabels class

Encapsule une collection de tous les objets DataLabel pour la série spécifiée.

```csharp
public class DataLabels : ChartTextFrame
```

## Propriétés

| Nom | La description |
| --- | --- |
| override [Area](../../aspose.cells.charts/datalabels/area) { get; } | Obtient le[`Région`](./area) . |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont) { get; set; } | True si le texte de l'objet change de taille de police lorsque la taille de l'objet change. La valeur par défaut est Vrai. |
| [BackgroundMode](../../aspose.cells.charts/datalabels/backgroundmode) { get; set; } | Obtient et définit le mode d'affichage de l'arrière-plan |
| override [Border](../../aspose.cells.charts/datalabels/border) { get; } | Obtient le[`frontière`](../../aspose.cells.drawing/line) . |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | Représente la hauteur de la position par défaut |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | Représente la largeur de la position par défaut |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | Représente x de la position par défaut |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | Représente y de la position par défaut |
| override [DirectionType](../../aspose.cells.charts/datalabels/directiontype) { get; set; } | Obtient et définit la direction du texte. |
| override [Font](../../aspose.cells.charts/datalabels/font) { get; } | Récupère la police des DataLabels ; |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | Obtient ou définit la hauteur du cadre en unités de 1/4000 de la zone du graphique. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Indique si le cadre du graphique est dimensionné automatiquement. |
| override [IsAutoText](../../aspose.cells.charts/datalabels/isautotext) { get; set; } | Indique que le texte est généré automatiquement. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Indique si la position par défaut (DefaultX, DefaultY, DefaultWidth et DefaultHeight) est définie. |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | Indique si ces étiquettes de données sont supprimées. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Indique si la taille de la zone de tracé comprend les graduations et les étiquettes d'axe. False spécifie que la taille doit déterminer la taille de la zone de tracé, les graduations et les étiquettes d'axe. |
| [IsNeverOverlap](../../aspose.cells.charts/datalabels/isneveroverlap) { get; set; } | Indique si les étiquettes de données ne se chevauchent jamais. (Pour le graphique à secteurs) |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | Obtient ou définit si une forme doit être ajustée automatiquement pour contenir entièrement le texte qui y est décrit. L'ajustement automatique est lorsque le texte d'une forme est mis à l'échelle afin de contenir tout le texte à l'intérieur. |
| override [IsTextWrapped](../../aspose.cells.charts/datalabels/istextwrapped) { get; set; } | Obtient ou définit une valeur indiquant si le texte est encapsulé. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | Obtient et définit une référence à la feuille de calcul. |
| [Number](../../aspose.cells.charts/datalabels/number) { get; set; } | Obtient et définit le format numérique intégré. |
| [NumberFormat](../../aspose.cells.charts/datalabels/numberformat) { get; set; } | Représente la chaîne de format de l'objet DataLabels. |
| [NumberFormatLinked](../../aspose.cells.charts/datalabels/numberformatlinked) { get; set; } | Vrai si le format des nombres est lié aux cellules (afin que le format des nombres change dans les libellés lorsqu'il change dans les cellules). |
| [Position](../../aspose.cells.charts/datalabels/position) { get; set; } | Représente la position de l'étiquette de données. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | Représente l'ordre de lecture du texte. |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | Représente l'angle de rotation du texte. |
| [SeparatorType](../../aspose.cells.charts/datalabels/separatortype) { get; set; } | Obtient ou définit le type de séparateur utilisé pour les étiquettes de données sur un graphique. |
| [SeparatorValue](../../aspose.cells.charts/datalabels/separatorvalue) { get; set; } | Obtient ou définit la valeur de séparateur utilisée pour les étiquettes de données sur un graphique. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | Vrai si le cadre a une ombre. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Obtient le[`ShapeProperties`](../chartframe/shapeproperties) objet. |
| [ShapeType](../../aspose.cells.charts/datalabels/shapetype) { get; set; } | Obtient ou définit le type de forme de l'étiquette de données. |
| [ShowBubbleSize](../../aspose.cells.charts/datalabels/showbubblesize) { get; set; } | Représente le comportement d'affichage de la valeur en pourcentage de l'étiquette de données d'un graphique spécifié. True affiche la valeur en pourcentage. Faux pour cacher. |
| [ShowCategoryName](../../aspose.cells.charts/datalabels/showcategoryname) { get; set; } | Représente le comportement d'affichage du nom de catégorie d'étiquette de données d'un graphique spécifié. True pour afficher le nom de catégorie des étiquettes de données d'un graphique. Faux pour masquer. |
| [ShowCellRange](../../aspose.cells.charts/datalabels/showcellrange) { get; set; } | Indique si la plage de cellules est affichée comme étiquettes de données. |
| [ShowLegendKey](../../aspose.cells.charts/datalabels/showlegendkey) { get; set; } | Représente le comportement d'affichage de la clé de légende de l'étiquette de données d'un graphique spécifié. Vrai si la clé de légende de l'étiquette de données est visible. |
| [ShowPercentage](../../aspose.cells.charts/datalabels/showpercentage) { get; set; } | Représente le comportement d'affichage de la valeur en pourcentage de l'étiquette de données d'un graphique spécifié. True affiche la valeur en pourcentage. Faux pour cacher. |
| [ShowSeriesName](../../aspose.cells.charts/datalabels/showseriesname) { get; set; } | Renvoie ou définit un booléen pour indiquer le comportement d'affichage du nom de la série pour les étiquettes de données sur un graphique. True pour afficher le nom de la série. Faux pour masquer. |
| [ShowValue](../../aspose.cells.charts/datalabels/showvalue) { get; set; } | Représente le comportement d'affichage des valeurs d'étiquette de données d'un graphique spécifié. True affiche les valeurs. Faux pour cacher. |
| override [Text](../../aspose.cells.charts/datalabels/text) { get; set; } | Obtient ou définit le texte de l'étiquette de données. |
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

// Définissez les DataLabels dans le graphique
DataLabels datalabels;
for (int i = 0; i  <chart.NSeries.Count; i++)
{
    datalabels = chart.NSeries[i].DataLabels;
    //Définir la position des DataLabels
    datalabels.Position = LabelPositionType.InsideBase;
    //Afficher le nom de la catégorie dans les DataLabels
    datalabels.ShowCategoryName = true;
    //Afficher la valeur dans les DataLabels
    datalabels.ShowValue = true;
    //Ne pas afficher le pourcentage dans les DataLabels
    datalabels.ShowPercentage = false;
    //Ne pas afficher la clé de légende.
    datalabels.ShowLegendKey = false;
}

[Visual Basic]

'Définir les DataLabels dans le graphique
Dim datalabels As DataLabels
Dim i As Integer
For i = 0 To chart.NSeries.Count - 1 Step 1
    datalabels = chart.NSeries(i).DataLabels
    'Définir la position des DataLabels
    datalabels.Position = LabelPositionType.InsideBase
    'Afficher le nom de la catégorie dans les DataLabels
    datalabels.ShowCategoryName= True
    'Afficher la valeur dans les DataLabels
    datalabels.ShowValue = True
    'Ne pas afficher le pourcentage dans les DataLabels
    datalabels.ShowPercentage = False
    'Ne pas afficher la clé de légende.
    datalabels.ShowLegendKey = False
Next
```

### Voir également

* class [ChartTextFrame](../charttextframe)
* espace de noms [Aspose.Cells.Charts](../../aspose.cells.charts)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
