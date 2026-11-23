---
title: "Axis.Bins"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Axis. Représente les intervalles sur un axe de graphique Histogramme/Pareto"
type: docs
url: /fr/net/aspose.cells.charts/axis/bins/
---
## Axis.Bins property

Représente les intervalles sur un axe de graphique (Histogramme/Pareto)

```csharp
public AxisBins Bins { get; }
```

### Remarques

Uniquement pour un graphique Histogramme ou Pareto.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyBinsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Données d'exemple
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Créer un histogramme
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Histogram, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A5", true);

            // Configurer les intervalles
            AxisBins bins = chart.ValueAxis.Bins;
            bins.IsAutomatic = false;
            bins.Width = 15;
            bins.Overflow = 55;
            bins.Underflow = 5;

            workbook.Save("AxisBinsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [AxisBins](../../axisbins/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


