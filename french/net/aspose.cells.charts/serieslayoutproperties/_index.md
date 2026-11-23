---
title: "Classe SeriesLayoutProperties"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.SeriesLayoutProperties class. Représente les propriétés de la disposition des séries"
type: docs
url: /fr/net/aspose.cells.charts/serieslayoutproperties/
---
## SeriesLayoutProperties class

Représente les propriétés de la disposition des séries.

```csharp
public class SeriesLayoutProperties
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [SeriesLayoutProperties](serieslayoutproperties/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [IsIntervalLeftClosed](../../aspose.cells.charts/serieslayoutproperties/isintervalleftclosed/) { get; set; } | Indique si l'intervalle est fermé du côté gauche. |
| [MapChartProjectionType](../../aspose.cells.charts/serieslayoutproperties/mapchartprojectiontype/) { get; set; } | Obtient et définit le type de projection de la carte. |
| [MapChartRegionType](../../aspose.cells.charts/serieslayoutproperties/mapchartregiontype/) { get; set; } | Obtient et définit le type de région de la carte. |
| [MapLabelLayout](../../aspose.cells.charts/serieslayoutproperties/maplabellayout/) { get; set; } | Obtient et définit la disposition des étiquettes de la carte. |
| [QuartileCalculation](../../aspose.cells.charts/serieslayoutproperties/quartilecalculation/) { get; set; } | Représente les propriétés statistiques de la série. |
| [ShowConnectorLines](../../aspose.cells.charts/serieslayoutproperties/showconnectorlines/) { get; set; } | Indique si les lignes de connexion sont affichées entre les points de données. |
| [ShowInnerPoints](../../aspose.cells.charts/serieslayoutproperties/showinnerpoints/) { get; set; } | Indique s'il faut afficher les points de données non aberrants. |
| [ShowMeanLine](../../aspose.cells.charts/serieslayoutproperties/showmeanline/) { get; set; } | Indique si la ligne reliant tous les points moyens doit être affichée. |
| [ShowMeanMarker](../../aspose.cells.charts/serieslayoutproperties/showmeanmarker/) { get; set; } | Indique si les marqueurs indiquant la moyenne sont affichés. |
| [ShowOutlierPoints](../../aspose.cells.charts/serieslayoutproperties/showoutlierpoints/) { get; set; } | Indique si les points de données aberrants sont affichés. |
| [Subtotals](../../aspose.cells.charts/serieslayoutproperties/subtotals/) { get; set; } | Représente l'index d'un point de données de sous-total. |

### Remarques

Applicable uniquement aux graphiques BoxWhisker, Funnel, ParetoLine, Sunburst, Treemap, Waterfall et Histogram.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesLayoutPropertiesDemo
    {
        public static void SeriesLayoutPropertiesExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
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

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ajouter des séries au graphique
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";
            Series series = chart.NSeries[seriesIndex];

            // Définir les valeurs de la série
            series.Values = "=B1:B4";

            // Accéder à l'objet SeriesLayoutProperties
            SeriesLayoutProperties layoutProperties = series.LayoutProperties;

            // Définir les propriétés de SeriesLayoutProperties
            layoutProperties.ShowConnectorLines = true;
            layoutProperties.ShowMeanLine = true;
            layoutProperties.ShowOutlierPoints = true;
            layoutProperties.ShowMeanMarker = true;
            layoutProperties.ShowInnerPoints = true;
            layoutProperties.QuartileCalculation = QuartileCalculationType.Inclusive;
            layoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;
            layoutProperties.IsIntervalLeftClosed = true;
            layoutProperties.MapChartRegionType = MapChartRegionType.World;
            layoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;

            // Enregistrez le classeur
            workbook.Save("SeriesLayoutPropertiesExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


