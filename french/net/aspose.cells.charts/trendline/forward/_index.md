---
title: "Trendline.Forward"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Trendline. Renvoie ou définit le nombre de périodes ou d'unités sur un graphique en nuage de points que la ligne de tendance prolonge vers l'avant. Le nombre de périodes doit être supérieur ou égal à zéro."
type: docs
url: /fr/net/aspose.cells.charts/trendline/forward/
---
## Trendline.Forward property

Renvoie ou définit le nombre de périodes (ou d'unités sur un graphique de dispersion) que la ligne de tendance étend vers l'avant. Le nombre de périodes doit être supérieur ou égal à zéro.

```csharp
public double Forward { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyForwardDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Ajouter un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Ajouter une ligne de tendance
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "Linear Trend";
            trendline.DisplayEquation = true;
            
            // Démontrer la propriété Forward
            trendline.Forward = 2.5; // Extend trendline forward by 2.5 units
            
            workbook.Save("TrendlineForwardDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


