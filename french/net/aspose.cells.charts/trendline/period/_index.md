---
title: "Trendline.Period"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Trendline. Renvoie ou définit la période pour la ligne de tendance moyenne mobile"
type: docs
url: /fr/net/aspose.cells.charts/trendline/period/
---
## Trendline.Period property

Renvoie ou définit la période pour la courbe de tendance moyenne mobile.

```csharp
public int Period { get; set; }
```

### Remarques

Cette valeur doit être comprise entre 2 et 255. Et elle doit être inférieure au nombre de points du graphique dans la série.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyPeriodDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
            }

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ajouter une série
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Ajouter une ligne de tendance moyenne mobile
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.MovingAverage);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Period = 3; // Set period for moving average
            trendline.Name = "3-Period Moving Average";

            // Enregistrez le classeur
            workbook.Save("TrendlinePeriodDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


