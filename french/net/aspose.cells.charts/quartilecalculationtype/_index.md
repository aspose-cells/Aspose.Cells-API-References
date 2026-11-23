---
title: "Enum QuartileCalculationType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.QuartileCalculationType enum. Représente les méthodes de calcul des quartiles"
type: docs
url: /fr/net/aspose.cells.charts/quartilecalculationtype/
---
## QuartileCalculationType enumeration

Représente les méthodes de calcul du quartile.

```csharp
public enum QuartileCalculationType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Exclusive | `0` | Le calcul des quartiles inclut la médiane lors de la division du jeu de données en quartiles. |
| Inclusive | `1` | Le calcul des quartiles exclut la médiane lors de la division du jeu de données en quartiles. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class QuartileCalculationTypeDemo
    {
        public static void QuartileCalculationTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 7, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Ajouter des séries au graphique
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Accédez aux propriétés de mise en page des séries
            SeriesLayoutProperties layoutProperties = chart.NSeries[0].LayoutProperties;

            // Définissez le type de calcul des quartiles
            layoutProperties.QuartileCalculation = QuartileCalculationType.Exclusive;

            // Enregistrez le classeur
            workbook.Save("QuartileCalculationTypeExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


