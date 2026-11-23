---
title: "Series.LeaderLines"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Représente les lignes de repère sur un graphique. Les lignes de repère relient les étiquettes de données aux points de données. Cet objet n’est pas une collection, il n’existe aucun objet représentant une seule ligne de repère"
type: docs
url: /fr/net/aspose.cells.charts/series/leaderlines/
---
## Series.LeaderLines property

Représente les lignes de repère sur un graphique. Les lignes de repère relient les étiquettes de données aux points de données. Cet objet n'est pas une collection ; il n'existe aucun objet représentant une seule ligne de repère.

```csharp
public Line LeaderLines { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyLeaderLinesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique en secteurs
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Configurer les étiquettes de données
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShowPercentage = true;
            series.DataLabels.Position = LabelPositionType.OutsideEnd;

            // Configurer les lignes de repère
            series.HasLeaderLines = true;
            series.LeaderLines.IsAuto = false;
            series.LeaderLines.Style = LineType.Dot;
            series.LeaderLines.WeightPt = 1.5;
            series.LeaderLines.Color = Color.Blue;

            // Enregistrez le classeur
            workbook.Save("SeriesPropertyLeaderLinesDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


