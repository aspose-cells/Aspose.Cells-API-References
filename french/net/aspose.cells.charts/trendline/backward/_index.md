---
title: "Trendline.Backward"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Trendline. Renvoie ou définit le nombre de périodes ou d'unités sur un graphique en nuage de points que la ligne de tendance prolonge vers l'arrière. Le nombre de périodes doit être supérieur ou égal à zéro. Si le type de graphique est en colonnes, le nombre de périodes doit être compris entre 0 et 0,5."
type: docs
url: /fr/net/aspose.cells.charts/trendline/backward/
---
## Trendline.Backward property

Renvoie ou définit le nombre de périodes (ou d'unités sur un graphique de dispersion) que la ligne de tendance étend vers l'arrière. Le nombre de périodes doit être supérieur ou égal à zéro. Si le type de graphique est en colonnes, le nombre de périodes doit être compris entre 0 et 0,5

```csharp
public double Backward { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyBackwardDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);

            // Ajouter une ligne de tendance et l'obtenir par indice
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(Aspose.Cells.Charts.TrendlineType.Linear);
            Aspose.Cells.Charts.Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "Linear Trend";
            trendline.DisplayEquation = true;
            
            // Définir la propriété Backward pour étendre la ligne de tendance vers l'arrière de 0,5 unité
            trendline.Backward = 0.5;
            
            workbook.Save("TrendlineBackwardDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


