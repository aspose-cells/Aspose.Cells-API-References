---
title: SparklineGroup
second_title: Référence de l'API Aspose.Cells pour .NET
description: Sparkline./sparkline est organisé en groupe sparkline. Un SparklineGroup contient un nombre variable déléments sparkline. Un groupe sparkline spécifie le type les paramètres daffichage et les paramètres daxe pour les sparklines.
type: docs
weight: 880
url: /fr/net/aspose.cells.charts/sparklinegroup/
---
## SparklineGroup class

[`Sparkline`](../sparkline) est organisé en groupe sparkline. Un SparklineGroup contient un nombre variable d'éléments sparkline. Un groupe sparkline spécifie le type, les paramètres d'affichage et les paramètres d'axe pour les sparklines.

```csharp
public class SparklineGroup
```

## Propriétés

| Nom | La description |
| --- | --- |
| [DisplayHidden](../../aspose.cells.charts/sparklinegroup/displayhidden) { get; set; } | Indique si les données doivent être affichées dans des lignes et des colonnes masquées. |
| [FirstPointColor](../../aspose.cells.charts/sparklinegroup/firstpointcolor) { get; set; } | Obtient et définit la couleur du premier point de données dans le groupe sparkline. |
| [HighPointColor](../../aspose.cells.charts/sparklinegroup/highpointcolor) { get; set; } | Obtient et définit la couleur des points de données les plus élevés dans le groupe sparkline. |
| [HorizontalAxisColor](../../aspose.cells.charts/sparklinegroup/horizontalaxiscolor) { get; set; } | Obtient et définit la couleur de l'axe horizontal dans le groupe sparkline. |
| [HorizontalAxisDateRange](../../aspose.cells.charts/sparklinegroup/horizontalaxisdaterange) { get; set; } | Représente la plage qui contient les valeurs de date pour les données sparkline. |
| [LastPointColor](../../aspose.cells.charts/sparklinegroup/lastpointcolor) { get; set; } | Obtient et définit la couleur du dernier point de données dans le groupe sparkline. |
| [LineWeight](../../aspose.cells.charts/sparklinegroup/lineweight) { get; set; } | Obtient et définit l'épaisseur de ligne dans chaque ligne sparkline du groupe de lignes sparkline, dans l'unité de points. |
| [LowPointColor](../../aspose.cells.charts/sparklinegroup/lowpointcolor) { get; set; } | Obtient et définit la couleur des points de données les plus bas dans le groupe sparkline. |
| [MarkersColor](../../aspose.cells.charts/sparklinegroup/markerscolor) { get; set; } | Obtient et définit la couleur des points dans chaque ligne sparkline du groupe sparkline. |
| [NegativePointsColor](../../aspose.cells.charts/sparklinegroup/negativepointscolor) { get; set; } | Obtient et définit la couleur des valeurs négatives sur le groupe sparkline. |
| [PlotEmptyCellsType](../../aspose.cells.charts/sparklinegroup/plotemptycellstype) { get; set; } | Indique comment tracer les cellules vides. |
| [PlotRightToLeft](../../aspose.cells.charts/sparklinegroup/plotrighttoleft) { get; set; } | Indique si les données du tracé sont de droite à gauche. |
| [PresetStyle](../../aspose.cells.charts/sparklinegroup/presetstyle) { get; set; } | Obtient et définit le type de style prédéfini du groupe sparkline. |
| [SeriesColor](../../aspose.cells.charts/sparklinegroup/seriescolor) { get; set; } | Obtient et définit la couleur des sparklines dans le groupe de sparklines. |
| [ShowFirstPoint](../../aspose.cells.charts/sparklinegroup/showfirstpoint) { get; set; } | Indique s'il faut mettre en surbrillance le premier point de données dans le groupe sparkline. |
| [ShowHighPoint](../../aspose.cells.charts/sparklinegroup/showhighpoint) { get; set; } | Indique s'il faut mettre en surbrillance les points de données les plus élevés dans le groupe sparkline. |
| [ShowHorizontalAxis](../../aspose.cells.charts/sparklinegroup/showhorizontalaxis) { get; set; } | Indique s'il faut afficher l'axe horizontal du graphique sparkline. L'axe horizontal apparaît si le graphique sparkline contient des données qui croisent l'axe zéro. |
| [ShowLastPoint](../../aspose.cells.charts/sparklinegroup/showlastpoint) { get; set; } | Indique s'il faut mettre en surbrillance le dernier point de données dans le groupe sparkline. |
| [ShowLowPoint](../../aspose.cells.charts/sparklinegroup/showlowpoint) { get; set; } | Indique s'il faut mettre en surbrillance les points de données les plus bas dans le groupe sparkline. |
| [ShowMarkers](../../aspose.cells.charts/sparklinegroup/showmarkers) { get; set; } | Indique s'il faut mettre en surbrillance chaque point de chaque ligne sparkline du groupe de lignes sparkline. |
| [ShowNegativePoints](../../aspose.cells.charts/sparklinegroup/shownegativepoints) { get; set; } | Indique s'il faut mettre en évidence les valeurs négatives sur le groupe sparkline avec une couleur ou un marqueur différent. |
| [SparklineCollection](../../aspose.cells.charts/sparklinegroup/sparklinecollection) { get; } | Obtient le[`SparklineCollection`](./sparklinecollection) objet du groupe sparkline. |
| [Type](../../aspose.cells.charts/sparklinegroup/type) { get; set; } | Indique le type de ligne sparkline du groupe de lignes sparkline. |
| [VerticalAxisMaxValue](../../aspose.cells.charts/sparklinegroup/verticalaxismaxvalue) { get; set; } | Obtient et définit la valeur maximale personnalisée pour l'axe vertical. |
| [VerticalAxisMaxValueType](../../aspose.cells.charts/sparklinegroup/verticalaxismaxvaluetype) { get; set; } | Représente le type de valeur maximale de l'axe vertical. |
| [VerticalAxisMinValue](../../aspose.cells.charts/sparklinegroup/verticalaxisminvalue) { get; set; } | Obtient et définit la valeur minimale personnalisée pour l'axe vertical. |
| [VerticalAxisMinValueType](../../aspose.cells.charts/sparklinegroup/verticalaxisminvaluetype) { get; set; } | Représente le type de valeur minimale de l'axe vertical. |

## Méthodes

| Nom | La description |
| --- | --- |
| [ResetRanges](../../aspose.cells.charts/sparklinegroup/resetranges)(string, bool, CellArea) | Réinitialise la plage de données et la plage d'emplacement du groupe sparkline. Cette méthode effacera les éléments sparkline d'origine du groupe et créera de nouveaux éléments sparkline pour les nouvelles plages. |

### Exemples

```csharp
[C#]
 Workbook book = new Workbook(); 
 Worksheet sheet = book.Worksheets[0];

 sheet.Cells["A1"].PutValue(5);
 sheet.Cells["B1"].PutValue(2);
 sheet.Cells["C1"].PutValue(1);
 sheet.Cells["D1"].PutValue(3);
 
 // Définir la CellArea
 CellArea ca = new CellArea();
 ca.StartColumn = 4;
 ca.EndColumn = 4;
 ca.StartRow = 0;
 ca.EndRow = 0;
 int idx = sheet.SparklineGroupCollection.Add(Aspose.Cells.Charts.SparklineType.Line, "A1:D1", false, ca);
 SparklineGroup group = sheet.SparklineGroupCollection[idx];
 group.SparklineCollection.Add(sheet.Name + "!A1:D1", 0, 4);
 // Créer une couleur de cellule
 CellsColor clr = book.CreateCellsColor();
 clr.Color = Color.Orange;
 group.SeriesColor = clr;

 // définit les points hauts sont colorés en vert et les points bas sont colorés en rouge
 group.ShowHighPoint = true;
 group.ShowLowPoint = true;
 group.HighPointColor.Color = Color.Green;
 group.LowPointColor.Color = Color.Red;
 // définit l'épaisseur de la ligne 
 group.LineWeight = 1.0;
 book.Save("output.xlsx", SaveFormat.Xlsx);
```

### Voir également

* espace de noms [Aspose.Cells.Charts](../../aspose.cells.charts)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
