---
title: "Trendline.DisplayEquation"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Trendline. Indique si l'équation de la courbe de tendance est affichée sur le graphique dans la même étiquette de données que la valeur R². Mettre cette propriété à True active automatiquement les étiquettes de données"
type: docs
url: /fr/net/aspose.cells.charts/trendline/displayequation/
---
## Trendline.DisplayEquation property

Indique si l'équation de la ligne de tendance est affichée sur le graphique (dans la même étiquette de données que la valeur R-carré). Définir cette propriété sur True active automatiquement les étiquettes de données.

```csharp
public bool DisplayEquation { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyDisplayEquationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);

            // Créer un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ajouter une série et une courbe de tendance
            chart.NSeries.Add("A1:B4", true);
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Configurer les propriétés de la courbe de tendance
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = false;
            trendline.Color = Color.Blue;

            workbook.Save("TrendlineDisplayEquationDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


