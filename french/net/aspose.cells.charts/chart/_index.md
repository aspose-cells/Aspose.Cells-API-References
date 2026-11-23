---
title: "Classe Chart"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Charts.Chart. Encapsule l'objet qui représente un graphique Excel unique."
type: docs
url: /fr/net/aspose.cells.charts/chart/
---
## Chart class

Encapsule l'objet qui représente un graphique Excel unique.

```csharp
public class Chart
```

## Propriétés

| Nom | Description |
| --- | --- |
| [ActualChartSize](../../aspose.cells.charts/chart/actualchartsize/) { get; } | (**Obsolete.**) Obtient la taille réelle du graphique en unités de pixels. |
| [AutoScaling](../../aspose.cells.charts/chart/autoscaling/) { get; set; } | Vrai si Microsoft Excel met à l'échelle un graphique 3D de manière à ce qu'il soit plus proche en taille du graphique 2D équivalent. La propriété RightAngleAxes doit être vraie. |
| [BackWall](../../aspose.cells.charts/chart/backwall/) { get; } | Renvoie un objet [`Walls`](./walls/) qui représente le mur arrière d'un graphique 3D. |
| [CategoryAxis](../../aspose.cells.charts/chart/categoryaxis/) { get; } | Obtient l'axe X du graphique. |
| [ChartArea](../../aspose.cells.charts/chart/chartarea/) { get; } | Obtient la zone du graphique dans la feuille de calcul. |
| [ChartDataTable](../../aspose.cells.charts/chart/chartdatatable/) { get; } | Représente le tableau de données du graphique. |
| [ChartObject](../../aspose.cells.charts/chart/chartobject/) { get; } | Représente le chartShape ; |
| [DepthPercent](../../aspose.cells.charts/chart/depthpercent/) { get; set; } | Représente la profondeur d'un graphique 3D en pourcentage de la largeur du graphique (entre 20 et 2000 pour cent). |
| [DisplayNaAsBlank](../../aspose.cells.charts/chart/displaynaasblank/) { get; set; } | Indique s'il faut afficher #N/A comme une valeur vide. |
| [Elevation](../../aspose.cells.charts/chart/elevation/) { get; set; } | Représente l'élévation de la vue du graphique 3D, en degrés. |
| [FilteredNSeries](../../aspose.cells.charts/chart/filterednseries/) { get; } | Obtient une collection [`SeriesCollection`](../seriescollection/) représentant les séries de données filtrées dans le graphique. |
| [FirstSliceAngle](../../aspose.cells.charts/chart/firstsliceangle/) { get; set; } | Obtient ou définit l'angle de la première tranche de diagramme circulaire ou de diagramme en anneau, en degrés (dans le sens des aiguilles d'une montre depuis la verticale). S'applique uniquement aux diagrammes circulaires, 3D circulaires et en anneau, de 0 à 360. |
| [Floor](../../aspose.cells.charts/chart/floor/) { get; } | Renvoie un objet [`Floor`](./floor/) qui représente les parois d'un graphique 3D. |
| [GapDepth](../../aspose.cells.charts/chart/gapdepth/) { get; set; } | Obtient ou définit la distance entre les séries de données dans un graphique 3D, en pourcentage de la largeur du marqueur. La valeur de cette propriété doit être comprise entre 0 et 500. |
| [GapWidth](../../aspose.cells.charts/chart/gapwidth/) { get; set; } | Renvoie ou définit l'espace entre les groupes de barres ou de colonnes, en pourcentage de la largeur de la barre ou de la colonne. La valeur de cette propriété doit être comprise entre 0 et 500. |
| [HeightPercent](../../aspose.cells.charts/chart/heightpercent/) { get; set; } | Renvoie ou définit la hauteur d'un graphique 3D en pourcentage de la largeur du graphique (entre 5 et 500 pour cent). |
| [HidePivotFieldButtons](../../aspose.cells.charts/chart/hidepivotfieldbuttons/) { get; set; } | Indique s'il faut masquer les boutons de champ du graphique croisé dynamique uniquement lorsque le graphique est un PivotChart. |
| [Is3D](../../aspose.cells.charts/chart/is3d/) { get; } | Indique si le graphique est un graphique 3D. |
| [IsRectangularCornered](../../aspose.cells.charts/chart/isrectangularcornered/) { get; set; } | Obtient ou définit une valeur indiquant si la zone du graphique a des coins rectangulaires. La valeur par défaut est true. |
| [Legend](../../aspose.cells.charts/chart/legend/) { get; } | Obtient la légende du graphique. |
| [Line](../../aspose.cells.charts/chart/line/) { get; } | Obtient la ligne. |
| [Name](../../aspose.cells.charts/chart/name/) { get; set; } | Obtient et définit le nom du graphique. |
| [NSeries](../../aspose.cells.charts/chart/nseries/) { get; } | Obtient une collection [`SeriesCollection`](../seriescollection/) représentant les séries de données du graphique. |
| [PageSetup](../../aspose.cells.charts/chart/pagesetup/) { get; } | Représente la description de la mise en page dans ce graphique. |
| [Perspective](../../aspose.cells.charts/chart/perspective/) { get; set; } | Renvoie ou définit la perspective de la vue du graphique tridimensionnel. Doit être comprise entre 0 et 100. Cette propriété est ignorée si la propriété RightAngleAxes est True. |
| [PivotOptions](../../aspose.cells.charts/chart/pivotoptions/) { get; } | Spécifie les contrôles de pivot qui apparaissent sur le graphique. |
| [PivotSource](../../aspose.cells.charts/chart/pivotsource/) { get; set; } | La source est les données du tableau croisé dynamique. Si PivotSource n'est pas vide, le graphique est un PivotChart. |
| [Placement](../../aspose.cells.charts/chart/placement/) { get; set; } | Représente la façon dont le graphique est attaché aux cellules en dessous. |
| [PlotArea](../../aspose.cells.charts/chart/plotarea/) { get; } | Obtient la zone de tracé du graphique qui comprend les étiquettes de graduation des axes. |
| [PlotBy](../../aspose.cells.charts/chart/plotby/) { get; } | Obtient et définit si le tracé se fait par ligne ou par colonne. |
| [PlotEmptyCellsType](../../aspose.cells.charts/chart/plotemptycellstype/) { get; set; } | Obtient et définit comment tracer les cellules vides. |
| [PlotVisibleCells](../../aspose.cells.charts/chart/plotvisiblecells/) { get; set; } | (**Obsolète.**) Indique si seules les cellules visibles du tracé sont prises en compte. |
| [PlotVisibleCellsOnly](../../aspose.cells.charts/chart/plotvisiblecellsonly/) { get; set; } | Indique si seules les cellules visibles du tracé le sont. |
| [PrintSize](../../aspose.cells.charts/chart/printsize/) { get; set; } | Obtient et définit la taille imprimée du graphique. |
| [RightAngleAxes](../../aspose.cells.charts/chart/rightangleaxes/) { get; set; } | Vrai si les axes du graphique sont perpendiculaires. S'applique uniquement aux graphiques 3D (sauf Column3D et graphiques 3D en secteurs). |
| [RotationAngle](../../aspose.cells.charts/chart/rotationangle/) { get; set; } | Représente la rotation de la vue du graphique 3D (la rotation de la zone du tracé autour de l'axe z, en degrés). |
| [SecondCategoryAxis](../../aspose.cells.charts/chart/secondcategoryaxis/) { get; } | Obtient le deuxième axe X du graphique. |
| [SecondValueAxis](../../aspose.cells.charts/chart/secondvalueaxis/) { get; } | Obtient le deuxième axe Y du graphique. |
| [SeriesAxis](../../aspose.cells.charts/chart/seriesaxis/) { get; } | Obtient l'axe des séries du graphique. |
| [Shapes](../../aspose.cells.charts/chart/shapes/) { get; } | Renvoie toutes les formes de dessin de ce graphique. |
| [ShowDataTable](../../aspose.cells.charts/chart/showdatatable/) { get; set; } | Obtient ou définit une valeur indiquant si le graphique affiche un tableau de données. |
| [ShowLegend](../../aspose.cells.charts/chart/showlegend/) { get; set; } | Obtient ou définit une valeur indiquant si la légende du graphique sera affichée. La valeur par défaut est vraie. |
| [SideWall](../../aspose.cells.charts/chart/sidewall/) { get; } | Renvoie un objet [`Walls`](./walls/) qui représente le mur latéral d'un graphique 3D. |
| [SizeWithWindow](../../aspose.cells.charts/chart/sizewithwindow/) { get; set; } | Vrai si Microsoft Excel redimensionne le graphique pour correspondre à la taille de la fenêtre de la feuille de graphique. |
| [Style](../../aspose.cells.charts/chart/style/) { get; set; } | Obtient et définit le style intégré. |
| [SubTitle](../../aspose.cells.charts/chart/subtitle/) { get; } | Obtient le sous-titre du graphique. S'applique uniquement aux fichiers ODS. |
| [Title](../../aspose.cells.charts/chart/title/) { get; } | Obtient le titre du graphique. |
| [Type](../../aspose.cells.charts/chart/type/) { get; set; } | Obtient ou définit le type d'un graphique. |
| [ValueAxis](../../aspose.cells.charts/chart/valueaxis/) { get; } | Obtient l'axe Y du graphique. |
| [Walls](../../aspose.cells.charts/chart/walls/) { get; } | Renvoie un objet [`Walls`](./walls/) qui représente les murs d'un graphique 3D. |
| [WallsAndGridlines2D](../../aspose.cells.charts/chart/wallsandgridlines2d/) { get; set; } | Vrai si les quadrillages sont dessinés en deux dimensions sur un graphique 3D. |
| [Worksheet](../../aspose.cells.charts/chart/worksheet/) { get; } | Obtient la feuille de calcul qui contient ce graphique. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Calculate](../../aspose.cells.charts/chart/calculate/#calculate)() | Calcule les positions personnalisées de la zone du tracé et des axes si leurs positions sont attribuées automatiquement. |
| [Calculate](../../aspose.cells.charts/chart/calculate/#calculate_1)(ChartCalculateOptions) | Calcule la position personnalisée de la zone du tracé et des axes si leur position est attribuée automatiquement, avec les options de calcul du graphique. |
| [ChangeTemplate](../../aspose.cells.charts/chart/changetemplate/)(byte[]) | Modifiez le type de graphique avec un modèle prédéfini. |
| [GetActualSize](../../aspose.cells.charts/chart/getactualsize/)() | Obtient la taille réelle du graphique en pixels. |
| [GetChartDataRange](../../aspose.cells.charts/chart/getchartdatarange/)() | Obtient la plage de source de données du graphique. |
| [HasAxis](../../aspose.cells.charts/chart/hasaxis/)(AxisType, bool) | Renvoie quels axes existent sur le graphique. |
| [IsCellReferedByChart](../../aspose.cells.charts/chart/iscellreferedbychart/)(int, int, int) | Renvoie si la cellule est référencée par le graphique. |
| [IsChartDataChanged](../../aspose.cells.charts/chart/ischartdatachanged/)() | Détecte si la source de données d'un graphique a changé. |
| [IsReferedByChart](../../aspose.cells.charts/chart/isreferedbychart/)(int, int) | (**Obsolete.**) Renvoie si la cellule est référencée par le graphique. |
| [Move](../../aspose.cells.charts/chart/move/)(int, int, int, int) | Déplace le graphique vers un emplacement spécifié. |
| [RefreshPivotData](../../aspose.cells.charts/chart/refreshpivotdata/)() | Actualise les données du graphique à partir du tableau croisé dynamique. |
| [SetChartDataRange](../../aspose.cells.charts/chart/setchartdatarange/)(string, bool) | Spécifie la plage de données pour un graphique. |
| [SwitchRowColumn](../../aspose.cells.charts/chart/switchrowcolumn/)() | Inverse les lignes/colonnes. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage)() | Obtient un objet `Bitmap` 32 bits du graphique. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_1)(ImageOrPrintOptions) | Obtient un objet `Bitmap` 32 bits du graphique. Les attributs `ImageOrPrintOptions.ImageFormat`, ImageOrPrintOptions.TiffCompression et ImageOrPrintOptions.Quality sont ignorés. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_6)(string) | Crée l'image du graphique et l'enregistre dans un fichier. L'extension du nom de fichier détermine le format de l'image. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_5)(Stream, ImageFormat) | (**Obsolete.**) Crée l'image du graphique et l'enregistre dans un flux au format spécifié. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_3)(Stream, ImageOrPrintOptions) | Crée l'image du graphique et l'enregistre dans un flux au format spécifié. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_2)(Stream, ImageType) | Crée l'image du graphique et l'enregistre dans un flux au format spécifié. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_4)(Stream, long) | Crée l'image du graphique et l'enregistre dans un flux au format Jpeg. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_10)(string, ImageFormat) | (**Obsolete.**) Crée l'image du graphique et l'enregistre dans un fichier au format spécifié. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_8)(string, ImageOrPrintOptions) | Crée l'image du graphique et l'enregistre dans un fichier. L'extension du nom de fichier détermine le format de l'image. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_7)(string, ImageType) | Crée l'image du graphique et l'enregistre dans un fichier au type d'image spécifié. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_9)(string, long) | (**Obsolete.**) Crée l'image du graphique et l'enregistre dans un fichier au format Jpeg. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf)(Stream) | Crée le PDF du graphique et l'enregistre dans un flux. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_2)(string) | Enregistre le graphique dans un fichier PDF. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_1)(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Crée le PDF du graphique et l'enregistre dans un flux. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_3)(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Enregistre le graphique dans un fichier PDF. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartDemo
    {
        public static void ChartExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells[0, 1].PutValue("Income");
            worksheet.Cells[1, 0].PutValue("Company A");
            worksheet.Cells[2, 0].PutValue("Company B");
            worksheet.Cells[3, 0].PutValue("Company C");
            worksheet.Cells[1, 1].PutValue(10000);
            worksheet.Cells[2, 1].PutValue(20000);
            worksheet.Cells[3, 1].PutValue(30000);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données pour le graphique
            chart.SetChartDataRange("A1:B4", true);

            // Définir les propriétés du graphique
            chart.ShowLegend = true;
            chart.Title.Text = "Income Analysis";
            chart.Style = 2; // Built-in style

            // Personnaliser l'apparence du graphique
            chart.ChartObject.Name = "IncomeChart";
            chart.PlotEmptyCellsType = PlotEmptyCellsType.NotPlotted;
            chart.PlotVisibleCells = true;
            chart.DisplayNaAsBlank = true;
            chart.SizeWithWindow = true;

            // Personnaliser les axes du graphique
            chart.CategoryAxis.Title.Text = "Companies";
            chart.ValueAxis.Title.Text = "Income";
            chart.CategoryAxis.MajorTickMark = TickMarkType.Outside;
            chart.ValueAxis.MajorTickMark = TickMarkType.Outside;

            // Personnaliser la légende du graphique
            chart.Legend.Position = LegendPositionType.Bottom;
            chart.Legend.IsOverLay = false;

            // Personnaliser la zone de tracé du graphique
            chart.PlotArea.Area.ForegroundColor = Color.LightYellow;
            chart.PlotArea.Border.IsVisible = false;

            // Personnaliser la zone du graphique
            chart.ChartArea.Area.ForegroundColor = Color.LightBlue;
            chart.ChartArea.Border.IsVisible = false;

            // Enregistrez le classeur
            workbook.Save("ChartExample.xlsx");
            workbook.Save("ChartExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


