---
title: "Trendline.DisplayRSquared"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Trendline. Indique si la valeur Rsquared de la ligne de tendance est affichée sur le graphique dans la même étiquette de données que l'équation. Définir cette propriété sur True active automatiquement les étiquettes de données."
type: docs
url: /fr/net/aspose.cells.charts/trendline/displayrsquared/
---
## Trendline.DisplayRSquared property

Indique si la valeur R-carré de la ligne de tendance est affichée sur le graphique (dans la même étiquette de données que l'équation). Définir cette propriété sur True active automatiquement les étiquettes de données.

```csharp
public bool DisplayRSquared { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyDisplayRSquaredDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].PutValue(4);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(6);
            worksheet.Cells["B4"].PutValue(8);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);

            // Ajouter une ligne de tendance et l'obtenir par indice
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "Linear Trend";
            
            // Démontrer la propriété DisplayRSquared
            trendline.DisplayRSquared = true;
            trendline.DisplayEquation = true;

            // Enregistrez le classeur
            workbook.Save("TrendlineDisplayRSquaredDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


