---
title: "TickLabels.IsAutomaticRotation"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TickLabels. Indique si l'angle de rotation est automatique"
type: docs
url: /fr/net/aspose.cells.charts/ticklabels/isautomaticrotation/
---
## TickLabels.IsAutomaticRotation property

Indique si l'angle de rotation est automatique

```csharp
public bool IsAutomaticRotation { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyIsAutomaticRotationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Ajouter un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configurer les étiquettes de graduation
            TickLabels tickLabels = chart.ValueAxis.TickLabels;
            tickLabels.IsAutomaticRotation = false; // Disable automatic rotation
            tickLabels.RotationAngle = 45; // Set manual rotation angle

            workbook.Save("TickLabelsRotationDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


