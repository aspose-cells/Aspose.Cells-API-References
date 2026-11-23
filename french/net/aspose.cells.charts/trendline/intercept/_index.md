---
title: "Trendline.Intercept"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Trendline. Retourne ou définit le point où la courbe de tendance croise l'axe des valeurs"
type: docs
url: /fr/net/aspose.cells.charts/trendline/intercept/
---
## Trendline.Intercept property

Renvoie ou définit le point où la ligne de tendance croise l'axe des valeurs.

```csharp
public double Intercept { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyInterceptDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(6);

            // Ajouter un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Ajouter une courbe de tendance et définir l'interception
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Intercept = 1.0; // Setting the Y-intercept value
            trendline.DisplayEquation = true;

            workbook.Save("TrendlineInterceptDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


