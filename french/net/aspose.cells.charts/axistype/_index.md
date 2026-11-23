---
title: "Enum AxisType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.AxisType enum. Représente le type d'axe"
type: docs
url: /fr/net/aspose.cells.charts/axistype/
---
## AxisType enumeration

Représente le type d'axe.

```csharp
public enum AxisType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Category | `0` | Axe de catégorie |
| Value | `1` | Axe de valeurs |
| Series | `2` | Axe de séries |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisTypeDemo
    {
        public static void AxisTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.SetChartDataRange("A1:B4", true);

            // Déterminez quels axes existent dans le graphique
            bool hasPrimaryCategoryAxis = chart.HasAxis(AxisType.Category, true);
            bool hasSecondaryCategoryAxis = chart.HasAxis(AxisType.Category, false);
            bool hasPrimaryValueAxis = chart.HasAxis(AxisType.Value, true);
            bool hasSecondaryValueAxis = chart.HasAxis(AxisType.Value, false);

            // Afficher les résultats
            Console.WriteLine("Has Primary Category Axis: " + hasPrimaryCategoryAxis);
            Console.WriteLine("Has Secondary Category Axis: " + hasSecondaryCategoryAxis);
            Console.WriteLine("Has Primary Value Axis: " + hasPrimaryValueAxis);
            Console.WriteLine("Has Secondary Value Axis: " + hasSecondaryValueAxis);

            // Enregistrez le classeur
            workbook.Save("AxisTypeExample.xlsx");
            workbook.Save("AxisTypeExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


