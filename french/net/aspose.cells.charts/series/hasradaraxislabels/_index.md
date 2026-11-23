---
title: "Series.HasRadarAxisLabels"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Vrai si un graphique radar possède des étiquettes d'axe de catégorie. S'applique uniquement aux graphiques radar"
type: docs
url: /fr/net/aspose.cells.charts/series/hasradaraxislabels/
---
## Series.HasRadarAxisLabels property

Vrai si un graphique radar possède des étiquettes d'axe de catégorie. S'applique uniquement aux graphiques radar.

```csharp
public bool HasRadarAxisLabels { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHasRadarAxisLabelsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple pour le graphique radar
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["A4"].PutValue("Cat3");
            
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(2);
            worksheet.Cells["B4"].PutValue(5);

            // Ajouter un graphique radar
            int chartIndex = worksheet.Charts.Add(ChartType.Radar, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ajouter des données de série
            int seriesIndex = chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtenez la série et définissez les étiquettes d'axe radar
            Series series = chart.NSeries[seriesIndex];
            series.HasRadarAxisLabels = true; // This is the key property being demonstrated

            // Enregistrez le classeur
            workbook.Save("RadarChartWithAxisLabels.xlsx");
        }
    }
}
```

### Voir aussi

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


