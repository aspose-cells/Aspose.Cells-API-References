---
title: "ErrorBar.Amount"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ErrorBar. Représente la quantité de la barre d'erreur"
type: docs
url: /fr/net/aspose.cells.charts/errorbar/amount/
---
## ErrorBar.Amount property

Représente la quantité de la barre d'erreur.

```csharp
public double Amount { get; set; }
```

### Remarques

La quantité doit être supérieure ou égale à zéro.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyAmountDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B1"].PutValue(15);
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["B3"].PutValue(35);

            // Créer un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configurer les barres d'erreur
            foreach (Series series in chart.NSeries)
            {
                series.YErrorBar.DisplayType = ErrorBarDisplayType.Both;
                series.YErrorBar.Type = ErrorBarType.FixedValue;
                series.YErrorBar.Amount = 5; // Demonstrate Amount property
            }

            workbook.Save("ErrorBarAmountDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


