---
title: "Classe DataLabels"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Charts.DataLabels. Encapsule une collection de tous les objets DataLabel pour la série spécifiée"
type: docs
url: /fr/net/aspose.cells.charts/datalabels/
---
## DataLabels class

Encapsule une collection de tous les objets DataLabel pour la Série spécifiée.

```csharp
public class DataLabels : ChartTextFrame
```

## Propriétés

| Nom | Description |
| --- | --- |
| override [Area](../../aspose.cells.charts/datalabels/area/) { get; } | Obtient le [`area`](./area/). |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont/) { get; set; } | Vrai si le texte de l'objet change de taille de police lorsque la taille de l'objet change. La valeur par défaut est Vrai.(Hérité de [`ChartFrame`](../chartframe/).) |
| [Background](../../aspose.cells.charts/chartframe/background/) { get; set; } | (**Obsolète.**) Obtient et définit le mode d'affichage de l'arrière-plan. Cette propriété n'est valide que dans Excel 2003 ou les versions antérieures.(Hérité de [`ChartFrame`](../chartframe/).) |
| [BackgroundMode](../../aspose.cells.charts/datalabels/backgroundmode/) { get; set; } | Obtient et définit le mode d'affichage de l'arrière-plan |
| override [Border](../../aspose.cells.charts/datalabels/border/) { get; } | Obtient le [`border`](../../aspose.cells.drawing/line/). |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight/) { get; } | (**Obsolète.**) Représente la hauteur de la position par défaut en unités de 1/4000 de la zone du graphique.(Hérité de [`ChartFrame`](../chartframe/).) |
| [DefaultHeightRatioToChart](../../aspose.cells.charts/chartframe/defaultheightratiotochart/) { get; } | Représente la hauteur de la position par défaut en unités de la fraction de la zone du graphique.(Hérité de [`ChartFrame`](../chartframe/).) |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth/) { get; } | (**Obsolète.**) Représente la largeur de la position par défaut en unités de 1/4000 de la zone du graphique.(Hérité de [`ChartFrame`](../chartframe/).) |
| [DefaultWidthRatioToChart](../../aspose.cells.charts/chartframe/defaultwidthratiotochart/) { get; } | Représente la largeur de la position par défaut en unités de la fraction de la zone du graphique.(Hérité de [`ChartFrame`](../chartframe/).) |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx/) { get; } | (**Obsolète.**) Représente x de la position par défaut en unités de 1/4000 de la zone du graphique.(Hérité de [`ChartFrame`](../chartframe/).) |
| [DefaultXRatioToChart](../../aspose.cells.charts/chartframe/defaultxratiotochart/) { get; } | Représente x de la position par défaut en unités de la fraction de la zone du graphique.(Hérité de [`ChartFrame`](../chartframe/).) |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty/) { get; } | (**Obsolète.**) Représente y de la position par défaut en unités de 1/4000 de la zone du graphique.(Hérité de [`ChartFrame`](../chartframe/).) |
| [DefaultYRatioToChart](../../aspose.cells.charts/chartframe/defaultyratiotochart/) { get; } | Représente y de la position par défaut en unités de la fraction de la zone du graphique.(Hérité de [`ChartFrame`](../chartframe/).) |
| override [DirectionType](../../aspose.cells.charts/datalabels/directiontype/) { get; set; } | Obtient et définit la direction du texte. |
| override [Font](../../aspose.cells.charts/datalabels/font/) { get; } | Obtient la police des DataLabels ; |
| virtual [Height](../../aspose.cells.charts/chartframe/height/) { get; set; } | (**Obsolete.**) Obtient ou définit la hauteur du cadre en unités de 1/4000 de la zone du graphique.(Hérité de [`ChartFrame`](../chartframe/).) |
| virtual [HeightPixel](../../aspose.cells.charts/chartframe/heightpixel/) { get; set; } | Obtient ou définit la hauteur du cadre en unités de pixels.(Hérité de [`ChartFrame`](../chartframe/).) |
| virtual [HeightRatioToChart](../../aspose.cells.charts/chartframe/heightratiotochart/) { get; set; } | Obtient ou définit la hauteur du cadre en unités du ratio de la zone du graphique.(Hérité de [`ChartFrame`](../chartframe/).) |
| [IsAutomaticRotation](../../aspose.cells.charts/charttextframe/isautomaticrotation/) { get; } | Indique si le texte du graphique est automatiquement pivoté.(Hérité de [`ChartTextFrame`](../charttextframe/).) |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize/) { get; set; } | Indique si le cadre du graphique est dimensionné automatiquement.(Hérité de [`ChartFrame`](../chartframe/).) |
| override [IsAutoText](../../aspose.cells.charts/datalabels/isautotext/) { get; set; } | Indique que le texte est généré automatiquement. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset/) { get; } | Indique si la position par défaut (DefaultX, DefaultY, DefaultWidth et DefaultHeight) est définie.(Hérité de [`ChartFrame`](../chartframe/).) |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted/) { get; set; } | Indique si cette étiquette de données est supprimée.(Hérité de [`ChartTextFrame`](../charttextframe/).) |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode/) { get; set; } | Indique si la taille de la zone de tracé inclut les marques de graduation et les étiquettes d'axe. False spécifie que la taille doit déterminer la taille de la zone de tracé, les marques de graduation et les étiquettes d'axe.(Hérité de [`ChartFrame`](../chartframe/).) |
| [IsNeverOverlap](../../aspose.cells.charts/datalabels/isneveroverlap/) { get; set; } | Indique si les étiquettes de données ne se chevauchent jamais lors de la conversion d’un diagramme circulaire en image. Remarque : cette propriété n’est pertinente que lors de la conversion d’un diagramme circulaire en image. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext/) { get; set; } | Obtient ou définit si une forme doit être ajustée automatiquement pour contenir entièrement le texte qui y est décrit. L'ajustement automatique consiste à mettre à l'échelle le texte à l'intérieur d'une forme afin d'y contenir tout le texte.(Hérité de [`ChartTextFrame`](../charttextframe/).) |
| override [IsTextWrapped](../../aspose.cells.charts/datalabels/istextwrapped/) { get; set; } | Obtient ou définit une valeur indiquant si le texte est renvoyé à la ligne. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource/) { get; set; } | Obtient et définit une référence à la feuille de calcul.(Hérité de [`ChartTextFrame`](../charttextframe/).) |
| [Number](../../aspose.cells.charts/datalabels/number/) { get; set; } | Obtient et définit le format de nombre intégré. |
| [NumberFormat](../../aspose.cells.charts/datalabels/numberformat/) { get; set; } | Représente la chaîne de format pour l'objet DataLabels. |
| [NumberFormatLinked](../../aspose.cells.charts/datalabels/numberformatlinked/) { get; set; } | Vrai si le format de nombre est lié aux cellules (de sorte que le format de nombre change dans les étiquettes lorsqu'il change dans les cellules). |
| [Position](../../aspose.cells.charts/datalabels/position/) { get; set; } | Représente la position de l'étiquette de données. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder/) { get; set; } | Représente l'ordre de lecture du texte.(Hérité de [`ChartTextFrame`](../charttextframe/).) |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle/) { get; set; } | Représente l'angle de rotation du texte.(Hérité de [`ChartTextFrame`](../charttextframe/).) |
| [SeparatorType](../../aspose.cells.charts/datalabels/separatortype/) { get; set; } | Obtient ou définit le type de séparateur utilisé pour les étiquettes de données sur un graphique. |
| [SeparatorValue](../../aspose.cells.charts/datalabels/separatorvalue/) { get; set; } | Obtient ou définit la valeur du séparateur utilisée pour les étiquettes de données sur un graphique. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow/) { get; set; } | Vrai si le cadre possède une ombre.(Hérité de [`ChartFrame`](../chartframe/).) |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties/) { get; } | Obtient l'objet [`ShapeProperties`](../chartframe/shapeproperties/).(Hérité de [`ChartFrame`](../chartframe/).) |
| [ShapeType](../../aspose.cells.charts/datalabels/shapetype/) { get; set; } | Obtient ou définit le type de forme de l'étiquette de données. |
| [ShowBubbleSize](../../aspose.cells.charts/datalabels/showbubblesize/) { get; set; } | Représente le comportement d'affichage de la valeur en pourcentage de l'étiquette de données d'un graphique spécifié. Vrai affiche la valeur en pourcentage. Faux masque la valeur en pourcentage. |
| [ShowCategoryName](../../aspose.cells.charts/datalabels/showcategoryname/) { get; set; } | Représente le comportement d'affichage du nom de catégorie de l'étiquette de données d'un graphique spécifié. Vrai pour afficher le nom de catégorie des étiquettes de données sur un graphique. Faux pour masquer. |
| [ShowCellRange](../../aspose.cells.charts/datalabels/showcellrange/) { get; set; } | Indique s'il faut afficher la plage de cellules comme étiquettes de données. |
| [ShowLegendKey](../../aspose.cells.charts/datalabels/showlegendkey/) { get; set; } | Représente le comportement d'affichage de la clé de légende de l'étiquette de données d'un graphique spécifié. Vrai si la clé de légende de l'étiquette de données est visible. |
| [ShowPercentage](../../aspose.cells.charts/datalabels/showpercentage/) { get; set; } | Représente le comportement d'affichage de la valeur en pourcentage de l'étiquette de données d'un graphique spécifié. Vrai affiche la valeur en pourcentage. Faux masque. |
| [ShowSeriesName](../../aspose.cells.charts/datalabels/showseriesname/) { get; set; } | Indique si le nom de la série s'affiche sur les étiquettes de données d'un graphique. Vrai pour afficher le nom de la série. Faux pour masquer. |
| [ShowValue](../../aspose.cells.charts/datalabels/showvalue/) { get; set; } | Représente le comportement d'affichage des valeurs de l'étiquette de données d'un graphique spécifié. Vrai affiche les valeurs. Faux masque. |
| override [Text](../../aspose.cells.charts/datalabels/text/) { get; set; } | Obtient ou définit le texte de l'étiquette de données. |
| [TextDirection](../../aspose.cells.charts/charttextframe/textdirection/) { get; set; } | (**Obsolete.**) Représente l'ordre de lecture du texte.(Hérité de [`ChartTextFrame`](../charttextframe/).) |
| virtual [TextFont](../../aspose.cells.charts/chartframe/textfont/) { get; } | (**Obsolete.**) Obtient un objet [`Font`](../chartframe/font/) du ChartFrame spécifié.(Hérité de [`ChartFrame`](../chartframe/).) |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment/) { get; set; } | Obtient et définit l'alignement horizontal du texte.(Hérité de [`ChartTextFrame`](../charttextframe/).) |
| virtual [TextOptions](../../aspose.cells.charts/chartframe/textoptions/) { get; } | Obtient et définit les options du texte.(Hérité de [`ChartFrame`](../chartframe/).) |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment/) { get; set; } | Obtient ou définit l'alignement vertical du texte.(Hérité de [`ChartTextFrame`](../charttextframe/).) |
| virtual [Width](../../aspose.cells.charts/chartframe/width/) { get; set; } | (**Obsolete.**) Obtient ou définit la largeur du cadre en unités de 1/4000 de la zone du graphique.(Hérité de [`ChartFrame`](../chartframe/).) |
| virtual [WidthPixel](../../aspose.cells.charts/chartframe/widthpixel/) { get; set; } | Obtient ou définit la largeur du cadre en unités de Pixel.(Hérité de [`ChartFrame`](../chartframe/).) |
| virtual [WidthRatioToChart](../../aspose.cells.charts/chartframe/widthratiotochart/) { get; set; } | Obtient ou définit la largeur du cadre en unités du rapport de la zone du graphique.(Hérité de [`ChartFrame`](../chartframe/).) |
| virtual [X](../../aspose.cells.charts/chartframe/x/) { get; set; } | (**Obsolete.**) Obtient ou définit la coordonnée x du coin supérieur gauche en unités de 1/4000 de la zone du graphique.(Hérité de [`ChartFrame`](../chartframe/).) |
| virtual [XPixel](../../aspose.cells.charts/chartframe/xpixel/) { get; set; } | Obtient ou définit la coordonnée x du coin supérieur gauche en unités de Pixel.(Hérité de [`ChartFrame`](../chartframe/).) |
| virtual [XRatioToChart](../../aspose.cells.charts/chartframe/xratiotochart/) { get; set; } | Obtient ou définit la coordonnée x du coin supérieur gauche en unités du ratio de la zone du graphique.(Hérité de [`ChartFrame`](../chartframe/).) |
| virtual [Y](../../aspose.cells.charts/chartframe/y/) { get; set; } | (**Obsolete.**) Obtient ou définit la coordonnée y du coin supérieur gauche en unités de 1/4000 de la zone du graphique.(Hérité de [`ChartFrame`](../chartframe/).) |
| virtual [YPixel](../../aspose.cells.charts/chartframe/ypixel/) { get; set; } | Obtient ou définit la coordonnée y du coin supérieur gauche en unités de pixels.(Hérité de [`ChartFrame`](../chartframe/).) |
| virtual [YRatioToChart](../../aspose.cells.charts/chartframe/yratiotochart/) { get; set; } | Obtient ou définit la coordonnée y du coin supérieur gauche en unités du ratio de la zone du graphique.(Hérité de [`ChartFrame`](../chartframe/).) |

## Méthodes

| Nom | Description |
| --- | --- |
| [ApplyFont](../../aspose.cells.charts/datalabels/applyfont/)() | Applique la police des étiquettes de données à tous les nœuds enfants. |
| [Characters](../../aspose.cells.charts/charttextframe/characters/)(int, int) | Renvoie un objet Characters qui représente une plage de caractères dans le texte.(Hérité de [`ChartTextFrame`](../charttextframe/).) |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto/)() | Définit la position du cadre sur automatique(Hérité de [`ChartFrame`](../chartframe/).) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class DataLabelsDemo
    {
        public static void DataLabelsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ajouter des séries au graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accédez aux DataLabels de la première série
            DataLabels dataLabels = chart.NSeries[0].DataLabels;

            // Définissez les propriétés des DataLabels
            dataLabels.Position = LabelPositionType.InsideBase;
            dataLabels.ShowCategoryName = true;
            dataLabels.ShowValue = true;
            dataLabels.ShowPercentage = false;
            dataLabels.ShowLegendKey = false;
            dataLabels.IsAutoText = true;
            dataLabels.DirectionType = ChartTextDirectionType.Horizontal;
            dataLabels.Text = "Custom Text";
            dataLabels.IsTextWrapped = true;
            dataLabels.BackgroundMode = BackgroundMode.Transparent;
            dataLabels.ShowCellRange = false;
            dataLabels.ShowBubbleSize = false;
            dataLabels.ShowSeriesName = false;
            dataLabels.NumberFormat = "0.00";
            dataLabels.Number = 0;
            dataLabels.NumberFormatLinked = false;
            dataLabels.SeparatorType = DataLabelsSeparatorType.Comma;
            dataLabels.SeparatorValue = ", ";
            dataLabels.IsNeverOverlap = true;
            dataLabels.IsDeleted = false;
            dataLabels.TextHorizontalAlignment = TextAlignmentType.Center;
            dataLabels.TextVerticalAlignment = TextAlignmentType.Center;
            dataLabels.RotationAngle = 0;
            dataLabels.LinkedSource = "";
            dataLabels.TextDirection = TextDirectionType.LeftToRight;
            dataLabels.ReadingOrder = TextDirectionType.LeftToRight;
            dataLabels.IsResizeShapeToFitText = true;
            dataLabels.IsInnerMode = false;
            dataLabels.AutoScaleFont = true;
            dataLabels.Background = BackgroundMode.Transparent;
            dataLabels.IsAutomaticSize = true;
            dataLabels.X = 0;
            dataLabels.Y = 0;
            dataLabels.Height = 100;
            dataLabels.Width = 100;
            dataLabels.Shadow = false;

            // Enregistrez le classeur
            workbook.Save("DataLabelsExample.xlsx");
            workbook.Save("DataLabelsExample.pdf");
        }
    }
}
```

### Voir aussi

* class [ChartTextFrame](../charttextframe/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


