---
title: Chart
second_title: Référence de l'API Aspose.Cells pour .NET
description: Encapsule lobjet qui représente un seul graphique Excel.
type: docs
weight: 430
url: /fr/net/aspose.cells.charts/chart/
---
## Chart class

Encapsule l'objet qui représente un seul graphique Excel.

```csharp
public class Chart
```

## Propriétés

| Nom | La description |
| --- | --- |
| [AutoScaling](../../aspose.cells.charts/chart/autoscaling) { get; set; } | Vrai si Microsoft Excel met à l'échelle un graphique 3D afin qu'il soit plus proche en taille du graphique 2D équivalent. La propriété RightAngleAxes doit être True. |
| [BackWall](../../aspose.cells.charts/chart/backwall) { get; } | Renvoie un[`Walls`](./walls) objet qui représente le mur arrière d'un graphique 3D. |
| [CategoryAxis](../../aspose.cells.charts/chart/categoryaxis) { get; } | Obtient l'axe X du graphique. |
| [ChartArea](../../aspose.cells.charts/chart/chartarea) { get; } | Obtient la zone de graphique dans la feuille de calcul. |
| [ChartDataTable](../../aspose.cells.charts/chart/chartdatatable) { get; } | Représente la table de données du graphique. |
| [ChartObject](../../aspose.cells.charts/chart/chartobject) { get; } | Représente la forme du graphique ; |
| [DepthPercent](../../aspose.cells.charts/chart/depthpercent) { get; set; } | Représente la profondeur d'un graphique 3D sous forme de pourcentage de la largeur du graphique (entre 20 et 2 000 %). |
| [DisplayNaAsBlank](../../aspose.cells.charts/chart/displaynaasblank) { get; set; } | Indique si #N/A est affiché comme valeur vide. |
| [Elevation](../../aspose.cells.charts/chart/elevation) { get; set; } | Représente l'élévation de la vue cartographique 3D, en degrés. |
| [FirstSliceAngle](../../aspose.cells.charts/chart/firstsliceangle) { get; set; } | Obtient ou définit l'angle de la première tranche de graphique à secteurs ou de graphique en anneau, en degrés (dans le sens des aiguilles d'une montre à partir de la verticale). S'applique uniquement aux graphiques à secteurs, à secteurs 3D et en anneau, de 0 à 360. |
| [Floor](../../aspose.cells.charts/chart/floor) { get; } | Renvoie un[`Floor`](./floor) objet qui représente les murs d'un graphique 3D. |
| [GapDepth](../../aspose.cells.charts/chart/gapdepth) { get; set; } | Obtient ou définit la distance entre les séries de données dans un graphique 3D, sous forme de pourcentage de la largeur du marqueur. La valeur de cette propriété doit être comprise entre 0 et 500. |
| [GapWidth](../../aspose.cells.charts/chart/gapwidth) { get; set; } | Renvoie ou définit l'espace entre les groupes de barres ou de colonnes, sous forme de pourcentage de la largeur de la barre ou de la colonne. La valeur de cette propriété doit être comprise entre 0 et 500. |
| [HeightPercent](../../aspose.cells.charts/chart/heightpercent) { get; set; } | Renvoie ou définit la hauteur d'un graphique 3D sous forme de pourcentage de la largeur du graphique (entre 5 et 500 %). |
| [HidePivotFieldButtons](../../aspose.cells.charts/chart/hidepivotfieldbuttons) { get; set; } | Indique si les boutons de champ du graphique croisé dynamique sont masqués uniquement lorsque le graphique est PivotChart. |
| [Is3D](../../aspose.cells.charts/chart/is3d) { get; } | Indique si le graphique est un graphique 3D. |
| [IsRectangularCornered](../../aspose.cells.charts/chart/isrectangularcornered) { get; set; } | Obtient ou définit une valeur indiquant si la zone du graphique est rectangulaire. La valeur par défaut est true. |
| [Legend](../../aspose.cells.charts/chart/legend) { get; } | Obtient la légende du graphique. |
| [Line](../../aspose.cells.charts/chart/line) { get; } | Obtient la ligne. |
| [Name](../../aspose.cells.charts/chart/name) { get; set; } | Obtient et définit le nom du graphique. |
| [NSeries](../../aspose.cells.charts/chart/nseries) { get; } | Obtient un[`SeriesCollection`](../seriescollection) collection représentant la série de données dans le graphique. |
| [PageSetup](../../aspose.cells.charts/chart/pagesetup) { get; } | Représente la description de la mise en page dans ce tableau. |
| [Perspective](../../aspose.cells.charts/chart/perspective) { get; set; } | Renvoie ou définit la perspective de la vue graphique 3D. Doit être compris entre 0 et 100. Cette propriété est ignorée si la propriété RightAngleAxes est True. |
| [PivotOptions](../../aspose.cells.charts/chart/pivotoptions) { get; } | Spécifie les contrôles de pivot qui apparaissent sur le graphique |
| [PivotSource](../../aspose.cells.charts/chart/pivotsource) { get; set; } | La source est les données du tableau croisé dynamique. Si PivotSource n'est pas vide, le graphique est PivotChart. |
| [Placement](../../aspose.cells.charts/chart/placement) { get; set; } | Représente la façon dont le graphique est attaché aux cellules en dessous. |
| [PlotArea](../../aspose.cells.charts/chart/plotarea) { get; } | Obtient la zone de tracé du graphique qui inclut les étiquettes de graduation des axes. |
| [PlotBy](../../aspose.cells.charts/chart/plotby) { get; } | Obtient et définit si le tracé est par ligne ou par colonne. |
| [PlotEmptyCellsType](../../aspose.cells.charts/chart/plotemptycellstype) { get; set; } | Obtient et définit comment tracer les cellules vides. |
| [PlotVisibleCells](../../aspose.cells.charts/chart/plotvisiblecells) { get; set; } | Indique si seules les cellules visibles sont tracées. |
| [PrintSize](../../aspose.cells.charts/chart/printsize) { get; set; } | Obtient et définit la taille du graphique imprimé. |
| [RightAngleAxes](../../aspose.cells.charts/chart/rightangleaxes) { get; set; } | Vrai si les axes du graphique sont à angle droit. S'applique uniquement aux graphiques 3D (sauf Column3D et 3-D Pie Charts). |
| [RotationAngle](../../aspose.cells.charts/chart/rotationangle) { get; set; } | Représente la rotation de la vue du graphique 3D (la rotation de la zone de tracé autour de l'axe z, en degrés). |
| [SecondCategoryAxis](../../aspose.cells.charts/chart/secondcategoryaxis) { get; } | Obtient le deuxième axe X du graphique. |
| [SecondValueAxis](../../aspose.cells.charts/chart/secondvalueaxis) { get; } | Obtient le deuxième axe Y du graphique. |
| [SeriesAxis](../../aspose.cells.charts/chart/seriesaxis) { get; } | Obtient l'axe des séries du graphique. |
| [Shapes](../../aspose.cells.charts/chart/shapes) { get; } | Renvoie toutes les formes de dessin dans ce graphique. |
| [ShowDataTable](../../aspose.cells.charts/chart/showdatatable) { get; set; } | Obtient ou définit une valeur indiquant si le graphique affiche une table de données. |
| [ShowLegend](../../aspose.cells.charts/chart/showlegend) { get; set; } | Obtient ou définit une valeur indiquant si la légende du graphique sera affichée. La valeur par défaut est true. |
| [SideWall](../../aspose.cells.charts/chart/sidewall) { get; } | Renvoie un[`Walls`](./walls)objet qui représente la paroi latérale d'un graphique 3D. |
| [SizeWithWindow](../../aspose.cells.charts/chart/sizewithwindow) { get; set; } | Vrai si Microsoft Excel redimensionne le graphique pour correspondre à la taille de la fenêtre de la feuille de graphique. |
| [Style](../../aspose.cells.charts/chart/style) { get; set; } | Obtient et définit le style intégré. |
| [SubTitle](../../aspose.cells.charts/chart/subtitle) { get; } | Récupère le sous-titre du graphique. Uniquement pour les fichiers au format ODS. |
| [Title](../../aspose.cells.charts/chart/title) { get; } | Obtient le titre du graphique. |
| [Type](../../aspose.cells.charts/chart/type) { get; set; } | Obtient ou définit le type d'un graphique. |
| [ValueAxis](../../aspose.cells.charts/chart/valueaxis) { get; } | Obtient l'axe Y du graphique. |
| [Walls](../../aspose.cells.charts/chart/walls) { get; } | Renvoie un[`Walls`](./walls) objet qui représente les murs d'un graphique 3D. |
| [WallsAndGridlines2D](../../aspose.cells.charts/chart/wallsandgridlines2d) { get; set; } | Vrai si le quadrillage est dessiné en deux dimensions sur un graphique 3D. |
| [Worksheet](../../aspose.cells.charts/chart/worksheet) { get; } | Obtient la feuille de calcul qui contient ce graphique. |

## Méthodes

| Nom | La description |
| --- | --- |
| [Calculate](../../aspose.cells.charts/chart/calculate)() | Calcule la position personnalisée de la zone de tracé, des axes si la position d'entre eux est attribuée automatiquement. |
| [GetActualSize](../../aspose.cells.charts/chart/getactualsize)() | Obtient la taille réelle du graphique en pixels. |
| [GetChartDataRange](../../aspose.cells.charts/chart/getchartdatarange)() | Obtient la plage de sources de données du graphique. |
| [HasAxis](../../aspose.cells.charts/chart/hasaxis)(AxisType, bool) | Renvoie les axes qui existent sur le graphique. |
| [IsChartDataChanged](../../aspose.cells.charts/chart/ischartdatachanged)() | Détecte si la source de données d'un graphique a changé. |
| [Move](../../aspose.cells.charts/chart/move)(int, int, int, int) | Déplace le graphique vers un emplacement spécifié. |
| [RefreshPivotData](../../aspose.cells.charts/chart/refreshpivotdata)() | Actualise les données du tableau croisé dynamique à partir de sa source de données pivot. |
| [SetChartDataRange](../../aspose.cells.charts/chart/setchartdatarange)(string, bool) | Spécifie la plage de données pour un graphique. |
| [SwitchRowColumn](../../aspose.cells.charts/chart/switchrowcolumn)() | Bascule ligne/colonne. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage)() | Obtient un 32 bits`Bitmap` objet du graphique. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_1)(ImageOrPrintOptions) | Obtient un 32 bits`Bitmap` objet du graphique. `ImageOrPrintOptions.ImageFormatImageOrPrintOptions.ImageFormat` , les attributs ImageOrPrintOptions.TiffCompression et ImageOrPrintOptions.Quality sont ignorés. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_6)(string) | Crée l'image du graphique et l'enregistre dans un fichier. L'extension du nom de fichier détermine le format de l'image. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_3)(Stream, ImageOrPrintOptions) | Crée l'image du graphique et l'enregistre dans un flux au format spécifié. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_2)(Stream, ImageType) | Crée l'image du graphique et l'enregistre dans un flux au format spécifié. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_4)(Stream, long) | Crée l'image du graphique et l'enregistre dans un flux au format Jpeg. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_8)(string, ImageOrPrintOptions) | Crée l'image du graphique et l'enregistre dans un fichier. L'extension du nom de fichier détermine le format de l'image. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_7)(string, ImageType) | Crée l'image du graphique et l'enregistre dans un fichier dans le type d'image spécifié. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_9)(string, long) | Crée l'image du graphique et l'enregistre dans un fichier au format Jpeg. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf)(Stream) | Crée le graphique pdf et l'enregistre dans un flux. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_2)(string) | Enregistre le graphique dans un fichier pdf. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_1)(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Crée le graphique pdf et l'enregistre dans un flux. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_3)(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Enregistre le graphique dans un fichier pdf. |

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
chart.ShowLegend = true;
chart.Title.Text = "Income Analysis";

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
chart.ShowLegend = True
chart.Title.Text = "Income Analysis"
```

### Voir également

* espace de noms [Aspose.Cells.Charts](../../aspose.cells.charts)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
