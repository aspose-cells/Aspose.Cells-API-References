---
title: "Classe ChartCalculateOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Charts.ChartCalculateOptions. Représente les options pour le calcul d'un graphique"
type: docs
url: /fr/net/aspose.cells.charts/chartcalculateoptions/
---
## ChartCalculateOptions class

Représente les options de calcul d'un graphique.

```csharp
public class ChartCalculateOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ChartCalculateOptions](chartcalculateoptions/)() | Crée les options pour le calcul du graphique. |

## Propriétés

| Nom | Description |
| --- | --- |
| [UpdateAllPoints](../../aspose.cells.charts/chartcalculateoptions/updateallpoints/) { get; set; } | Indique s'il faut mettre à jour tous les points de données lors du calcul du graphique. Valeur par défaut : False. Lorsque vous souhaitez obtenir la valeur de chaque point de données du graphique spécifiquement, réglez-le sur true. Si ce paramètre est défini sur True, de nouveaux points de données peuvent être générés lors du calcul du graphique. Cela peut augmenter la taille du fichier Excel. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCalculateOptionsDemo
    {
        public static void ChartCalculateOptionsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données pour le graphique
            chart.SetChartDataRange("A1:B4", true);

            // Créer une instance de ChartCalculateOptions
            ChartCalculateOptions options = new ChartCalculateOptions
            {
                UpdateAllPoints = true // Set the property to update all data points
            };

            // Calculer le graphique avec les options spécifiées
            chart.Calculate(options);

            // Enregistrez le classeur
            workbook.Save("ChartCalculateOptionsExample.xlsx");
            workbook.Save("ChartCalculateOptionsExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


