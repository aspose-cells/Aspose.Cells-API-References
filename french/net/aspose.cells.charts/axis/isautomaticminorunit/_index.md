---
title: "Axis.IsAutomaticMinorUnit"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Axis. Indique si l'unité mineure de l'axe est attribuée automatiquement"
type: docs
url: /fr/net/aspose.cells.charts/axis/isautomaticminorunit/
---
## Axis.IsAutomaticMinorUnit property

Indique si l'unité secondaire de l'axe est attribuée automatiquement.

```csharp
public bool IsAutomaticMinorUnit { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsAutomaticMinorUnitDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Obtenir l'axe des valeurs
            Axis valueAxis = chart.ValueAxis;

            // Démontrer la propriété IsAutomaticMinorUnit
            Console.WriteLine("Initial IsAutomaticMinorUnit: " + valueAxis.IsAutomaticMinorUnit);
            
            // Définir l'unité mineure manuellement
            valueAxis.IsAutomaticMinorUnit = false;
            valueAxis.MinorUnit = 2;
            Console.WriteLine("After setting manually - IsAutomaticMinorUnit: " + valueAxis.IsAutomaticMinorUnit);
            Console.WriteLine("MinorUnit: " + valueAxis.MinorUnit);

            // Revenir à automatique
            valueAxis.IsAutomaticMinorUnit = true;
            Console.WriteLine("After setting automatic - IsAutomaticMinorUnit: " + valueAxis.IsAutomaticMinorUnit);

            // Enregistrez le classeur
            workbook.Save("AxisPropertyIsAutomaticMinorUnitDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


