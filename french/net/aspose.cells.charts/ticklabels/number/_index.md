---
title: "TickLabels.Number"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TickLabels. Représente le numéro de format pour l'objet TickLabels"
type: docs
url: /fr/net/aspose.cells.charts/ticklabels/number/
---
## TickLabels.Number property

Représente le numéro de format pour l'objet TickLabels.

```csharp
public int Number { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyNumberDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Configurer les étiquettes de graduation
            TickLabels tickLabels = chart.ValueAxis.TickLabels;
            tickLabels.Number = 2; // Demonstrate Number property
            tickLabels.NumberFormat = "0.00";

            // Enregistrez le classeur
            workbook.Save("TickLabelsNumberDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


