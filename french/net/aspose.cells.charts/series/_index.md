---
title: "Classe Series"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.Series class. Encapsule l'objet qui représente une série de données unique dans un graphique"
type: docs
url: /fr/net/aspose.cells.charts/series/
---
## Series class

Encapsule l'objet qui représente une série de données unique dans un graphique.

```csharp
public class Series
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Area](../../aspose.cells.charts/series/area/) { get; } | Représente la zone d'arrière-plan de l'objet Series. |
| [Bar3DShapeType](../../aspose.cells.charts/series/bar3dshapetype/) { get; set; } | Obtient ou définit le type de forme 3D utilisé avec le graphique à barres ou colonnes 3D. |
| [Border](../../aspose.cells.charts/series/border/) { get; } | Représente la bordure d'un objet Series. |
| [BubbleScale](../../aspose.cells.charts/series/bubblescale/) { get; set; } | Obtient ou définit le facteur d'échelle des bulles dans le groupe de graphiques spécifié. Il peut s'agir d'une valeur entière de 0 (zéro) à 300, correspondant à un pourcentage de la taille par défaut. S'applique uniquement aux graphiques à bulles. |
| [BubbleSizes](../../aspose.cells.charts/series/bubblesizes/) { get; set; } | Obtient ou définit les valeurs de taille des bulles de la série du graphique. |
| [CachedCategoryValues](../../aspose.cells.charts/series/cachedcategoryvalues/) { get; } | (**Obsolete.**) Obtient les valeurs de catégorie mises en cache pour la série |
| [CachedValues](../../aspose.cells.charts/series/cachedvalues/) { get; } | (**Obsolete.**) Obtient les valeurs mises en cache pour la série |
| [CategoryValues](../../aspose.cells.charts/series/categoryvalues/) { get; } | Obtient les valeurs de catégorie réelles utilisées pour tracer chaque point de cette série dans le graphique. |
| [CountOfDataValues](../../aspose.cells.charts/series/countofdatavalues/) { get; } | Obtient le nombre de valeurs de données. |
| [DataLabels](../../aspose.cells.charts/series/datalabels/) { get; } | Représente l'objet DataLabels pour la ASeries spécifiée. |
| [DisplayName](../../aspose.cells.charts/series/displayname/) { get; } | Obtient le nom de la série affiché sur le graphique. |
| [DoughnutHoleSize](../../aspose.cells.charts/series/doughnutholesize/) { get; set; } | Renvoie ou définit la taille du trou dans un groupe de graphique en anneau. La taille du trou est exprimée en pourcentage de la taille du graphique, entre 10 et 90 %. |
| [DownBars](../../aspose.cells.charts/series/downbars/) { get; } | Renvoie un objet [`DropBars`](../dropbars/) qui représente les barres descendantes sur un graphique en courbes. S'applique uniquement aux graphiques en courbes. |
| [DropLines](../../aspose.cells.charts/series/droplines/) { get; } | Renvoie un objet [`Line`](../../aspose.cells.drawing/line/) qui représente les lignes de chute pour une série sur le graphique en courbes ou le graphique en aires. S'applique uniquement aux graphiques en courbes ou aux graphiques en aires. |
| [Explosion](../../aspose.cells.charts/series/explosion/) { get; set; } | La distance d'une tranche de secteur ouverte du centre du graphique en secteurs est exprimée en pourcentage du diamètre du secteur. |
| [FirstSliceAngle](../../aspose.cells.charts/series/firstsliceangle/) { get; set; } | Obtient ou définit l'angle de la première tranche de graphique circulaire ou d'anneau, en degrés (dans le sens des aiguilles d'une montre depuis la verticale). S'applique uniquement aux graphiques circulaires, 3D circulaires et en anneau, avec des valeurs de 0 à 360. |
| [GapWidth](../../aspose.cells.charts/series/gapwidth/) { get; set; } | Renvoie ou définit l'espace entre les groupes de barres ou de colonnes, en pourcentage de la largeur de la barre ou de la colonne. La valeur de cette propriété doit être comprise entre 0 et 500. |
| [Has3DEffect](../../aspose.cells.charts/series/has3deffect/) { get; set; } | Vrai si la série a un aspect tridimensionnel. |
| [HasDropLines](../../aspose.cells.charts/series/hasdroplines/) { get; set; } | Vrai si le graphique possède des lignes de chute. S'applique uniquement aux graphiques en courbes ou aux graphiques en aires. |
| [HasHiLoLines](../../aspose.cells.charts/series/hashilolines/) { get; set; } | Vrai si le graphique en courbes possède des lignes haut-bas. S'applique uniquement aux graphiques en courbes. |
| [HasLeaderLines](../../aspose.cells.charts/series/hasleaderlines/) { get; set; } | Vrai si la série possède des lignes de repère. |
| [HasRadarAxisLabels](../../aspose.cells.charts/series/hasradaraxislabels/) { get; set; } | Vrai si un graphique radar possède des étiquettes d'axe de catégorie. S'applique uniquement aux graphiques radar. |
| [HasSeriesLines](../../aspose.cells.charts/series/hasserieslines/) { get; set; } | Vrai si un graphique à colonnes empilées ou à barres possède des lignes de séries ou si un graphique « Pie of Pie » ou « Bar of Pie » possède des lignes de connexion entre les deux sections. S'applique uniquement aux graphiques à colonnes empilées, à barres, « Pie of Pie » ou « Bar of Pie ». |
| [HasUpDownBars](../../aspose.cells.charts/series/hasupdownbars/) { get; set; } | Vrai si un graphique en courbes possède des barres haut et bas. S'applique uniquement aux graphiques en courbes. |
| [HiLoLines](../../aspose.cells.charts/series/hilolines/) { get; } | Renvoie un objet HiLoLines qui représente les lignes haut-bas pour une série sur un graphique en courbes. S'applique uniquement aux graphiques en courbes. |
| [IsAutoSplit](../../aspose.cells.charts/series/isautosplit/) { get; } | Indique si la valeur du seuil est automatique. |
| [IsColorVaried](../../aspose.cells.charts/series/iscolorvaried/) { get; set; } | Indique si la couleur des points varie. Le graphique doit contenir une seule série ou être un graphique circulaire. |
| [IsFiltered](../../aspose.cells.charts/series/isfiltered/) { get; set; } | Indique si la série est sélectionnée ou filtrée. Vrai indique que cette série est filtrée et ne sera pas affichée sur le graphique. |
| [IsVerticalValues](../../aspose.cells.charts/series/isverticalvalues/) { get; } | Indique si la source de données est verticale. |
| [LayoutProperties](../../aspose.cells.charts/series/layoutproperties/) { get; } | Représente les propriétés de la mise en page. |
| [LeaderLines](../../aspose.cells.charts/series/leaderlines/) { get; } | Représente les lignes de repère sur un graphique. Les lignes de repère relient les étiquettes de données aux points de données. Cet objet n'est pas une collection ; il n'existe aucun objet représentant une seule ligne de repère. |
| [LegendEntry](../../aspose.cells.charts/series/legendentry/) { get; } | Obtient l'entrée de légende correspondant à cette série. |
| [Marker](../../aspose.cells.charts/series/marker/) { get; } | Obtient le [`marker`](./marker/). |
| [Name](../../aspose.cells.charts/series/name/) { get; set; } | Obtient ou définit le nom de la série de données. |
| [Overlap](../../aspose.cells.charts/series/overlap/) { get; set; } | Spécifie comment les barres et colonnes sont positionnées. Peut être une valeur entre -100 et 100. S'applique uniquement aux graphiques à barres 2D et à colonnes 2D. |
| [PlotOnSecondAxis](../../aspose.cells.charts/series/plotonsecondaxis/) { get; set; } | Indique si cette série est tracée sur le deuxième axe des valeurs. |
| [Points](../../aspose.cells.charts/series/points/) { get; } | Obtient la collection de points d'une série dans un graphique. |
| [PointValues](../../aspose.cells.charts/series/pointvalues/) { get; } | Obtient les valeurs réelles utilisées pour tracer chaque point de cette série dans le graphique. |
| [SecondPlotSize](../../aspose.cells.charts/series/secondplotsize/) { get; set; } | Renvoie ou définit la taille de la section secondaire d'un graphique en secteurs de secteurs ou d'un graphique en barres de secteurs, en pourcentage de la taille du secteur principal. Peut être une valeur de 5 à 200. |
| [SeriesLines](../../aspose.cells.charts/series/serieslines/) { get; } | Renvoie un objet SeriesLines qui représente les lignes de série pour un graphique à barres empilées ou un graphique à colonnes empilées. S'applique uniquement aux graphiques à barres empilées et à colonnes empilées. |
| [Shadow](../../aspose.cells.charts/series/shadow/) { get; set; } | Vrai si la série possède une ombre. |
| [ShapeProperties](../../aspose.cells.charts/series/shapeproperties/) { get; } | Obtient l'objet [`ShapePropertyCollection`](../../aspose.cells.drawing/shapepropertycollection/) qui contient les propriétés visuelles de forme de la série. |
| [ShowNegativeBubbles](../../aspose.cells.charts/series/shownegativebubbles/) { get; set; } | Vrai si les bulles négatives sont affichées pour le groupe de graphique. Valide uniquement pour les graphiques à bulles. |
| [SizeRepresents](../../aspose.cells.charts/series/sizerepresents/) { get; set; } | Obtient ou définit ce que représente la taille de la bulle dans un graphique à bulles. |
| [Smooth](../../aspose.cells.charts/series/smooth/) { get; set; } | Représente le lissage de courbe. Vrai si le lissage de courbe est activé pour le graphique en lignes ou le nuage de points. S'applique uniquement aux graphiques en lignes et aux nuages de points avec lignes. |
| [SplitType](../../aspose.cells.charts/series/splittype/) { get; set; } | Renvoie ou définit une valeur qui détermine quels points de données se trouvent dans le deuxième secteur ou la deuxième barre d'un graphique en secteurs de secteurs ou en barres de secteurs. |
| [SplitValue](../../aspose.cells.charts/series/splitvalue/) { get; set; } | Renvoie ou définit une valeur qui sera utilisée pour déterminer quels points de données se trouvent dans le deuxième secteur ou la deuxième barre d'un graphique en secteurs de secteurs ou en barres de secteurs. |
| [TrendLines](../../aspose.cells.charts/series/trendlines/) { get; } | Renvoie toutes les lignes de tendance de cette série. |
| [Type](../../aspose.cells.charts/series/type/) { get; set; } | Obtient ou définit le type d'une série de données. |
| [UpBars](../../aspose.cells.charts/series/upbars/) { get; } | Renvoie un objet DropBars qui représente les barres ascendantes sur un graphique en lignes. S'applique uniquement aux graphiques en lignes. |
| [Values](../../aspose.cells.charts/series/values/) { get; set; } | Représente les valeurs Y de cette série de graphique. |
| [ValuesFormatCode](../../aspose.cells.charts/series/valuesformatcode/) { get; set; } | Représente le code de format de la liste de nombres des valeurs. |
| [XErrorBar](../../aspose.cells.charts/series/xerrorbar/) { get; } | Représente la barre d'erreur en direction X de la série. |
| [XValues](../../aspose.cells.charts/series/xvalues/) { get; set; } | Représente les valeurs X de cette série de graphique. |
| [XValuesFormatCode](../../aspose.cells.charts/series/xvaluesformatcode/) { get; set; } | Représente le code de format de la liste de nombres des valeurs X. |
| [YErrorBar](../../aspose.cells.charts/series/yerrorbar/) { get; } | Représente la barre d'erreur en direction Y de la série. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Move](../../aspose.cells.charts/series/move/)(int) | Déplace la série vers le haut ou vers le bas. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesDemo
    {
        public static void SeriesExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();
            // Ajout d'une nouvelle feuille de calcul à l'objet Excel
            int sheetIndex = workbook.Worksheets.Add();
            // Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son indice de feuille
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Ajout de valeurs d'exemple aux cellules
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Ajout d'un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            // Accès à l'instance du graphique nouvellement ajouté
            Chart chart = worksheet.Charts[chartIndex];
            // Ajoute NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "B4"
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            // Définir la source de données pour les données de catégorie de NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // Accéder à la série
            Series series = chart.NSeries[seriesIndex];

            // Définir les valeurs de la série
            series.Values = "=B1:B4";
            // Modifier le type de graphique de la série
            series.Type = ChartType.Line;
            // Définir les propriétés du marqueur
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.ForegroundColorSetType = FormattingType.Automatic;
            series.Marker.ForegroundColor = System.Drawing.Color.Black;
            series.Marker.BackgroundColorSetType = FormattingType.Automatic;

            // Définition de propriétés supplémentaires
            series.Name = "First Series";
            series.IsFiltered = false;
            series.ValuesFormatCode = "0.00";
            series.XValues = "=A1:A4";
            series.BubbleSizes = "=B1:B4";
            series.Smooth = true;
            series.Shadow = true;
            series.Has3DEffect = true;
            series.Bar3DShapeType = Bar3DShapeType.Cylinder;
            series.PlotOnSecondAxis = false;
            series.HasHiLoLines = false;
            series.HasSeriesLines = false;
            series.HasDropLines = false;
            series.HasUpDownBars = false;
            series.IsColorVaried = false;
            series.GapWidth = 150;
            series.FirstSliceAngle = 45;
            series.Overlap = 0;
            series.SecondPlotSize = 100;
            series.SplitType = ChartSplitType.Position;
            series.SplitValue = 10.0;
            series.BubbleScale = 100;
            series.SizeRepresents = BubbleSizeRepresents.SizeIsArea;
            series.ShowNegativeBubbles = true;
            series.DoughnutHoleSize = 50;
            series.Explosion = 10;
            series.HasRadarAxisLabels = false;
            series.HasLeaderLines = true;

            // Enregistrement du fichier Excel
            workbook.Save("SeriesExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


