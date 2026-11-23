---
title: "ChartPoint.IsInSecondaryPlot"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartPoint. Obtient ou définit une valeur indiquant si ce point de données se trouve dans le deuxième diagramme circulaire ou barre d'un graphique circulaire imbriqué ou d'un graphique barre imbriqué"
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/isinsecondaryplot/
---
## ChartPoint.IsInSecondaryPlot property

Obtient ou définit une valeur indiquant si ce point de données se trouve dans le deuxième secteur ou barre d'un diagramme pie of pie ou bar of pie.

```csharp
public bool IsInSecondaryPlot { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyIsInSecondaryPlotDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Créer un diagramme circulaire qui prend en charge les tracés secondaires
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configurer le tracé secondaire
            chart.NSeries[0].Points[2].IsInSecondaryPlot = true;
            chart.NSeries[0].Points[3].IsInSecondaryPlot = true;

            // Enregistrer la sortie
            workbook.Save("PieChartWithSecondaryPlot.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


