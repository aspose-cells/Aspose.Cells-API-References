---
title: "Enum TimeUnit"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.TimeUnit enum. Représente l'unité de base pour l'axe de catégorie"
type: docs
url: /fr/net/aspose.cells.charts/timeunit/
---
## TimeUnit enumeration

Représente l'unité de base pour l'axe des catégories.

```csharp
public enum TimeUnit
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Days | `0` | Jours |
| Months | `1` | Mois |
| Years | `2` | Années |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TimeUnitDemo
    {
        public static void TimeUnitExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            // Ajouter une nouvelle feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["B1"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["B3"].PutValue(300);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Ajouter des séries au graphique
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Définissez l'axe de catégorie pour utiliser des unités de temps
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.CategoryType = CategoryType.TimeScale;
            categoryAxis.BaseUnitScale = TimeUnit.Months;
            categoryAxis.MajorUnitScale = TimeUnit.Months;
            categoryAxis.MinorUnitScale = TimeUnit.Days;

            // Personnalisez l'apparence du graphique
            chart.Title.Text = "Sample Chart with Time Units";
            chart.ValueAxis.Title.Text = "Values";
            chart.CategoryAxis.Title.Text = "Dates";

            // Enregistrez le classeur
            workbook.Save("TimeUnitExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


