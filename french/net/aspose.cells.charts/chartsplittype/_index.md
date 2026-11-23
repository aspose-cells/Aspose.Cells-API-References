---
title: "Enum ChartSplitType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.ChartSplitType enum. Représente la façon dont les deux sections d'un graphique en secteurs de secteurs ou d'un graphique en barres de secteurs sont séparées"
type: docs
url: /fr/net/aspose.cells.charts/chartsplittype/
---
## ChartSplitType enumeration

Représente la façon dont les deux sections d'un graphique en secteur de secteur ou d'un graphique en barre de secteur sont séparées.

```csharp
public enum ChartSplitType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Position | `0` | Représente les points de données. Les points de données doivent être répartis entre le secteur et le deuxième graphique en plaçant la dernière position de division des points de données dans le deuxième graphique. |
| Value | `1` | Représente les points de données qui doivent être répartis entre le secteur et le deuxième graphique en plaçant les points de données dont la valeur est inférieure à la position de division dans le deuxième graphique. |
| PercentValue | `2` | Représente les points de données qui doivent être répartis entre le secteur et le deuxième graphique en plaçant les points dont le pourcentage est inférieur au pourcentage de position de division dans le deuxième graphique. |
| Custom | `3` | Représente les points de données qui doivent être répartis entre le secteur et le deuxième graphique selon les valeurs de division personnalisées. |
| Auto | `4` | Représente les points de données qui doivent être répartis en utilisant le mécanisme par défaut pour ce type de graphique. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartsClassChartSplitTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ajouter des données d'exemple pour le graphique
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["A2"].PutValue("A");
                worksheet.Cells["A3"].PutValue("B");
                worksheet.Cells["A4"].PutValue("C");
                worksheet.Cells["A5"].PutValue("D");

                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["B3"].PutValue(20);
                worksheet.Cells["B4"].PutValue(30);
                worksheet.Cells["B5"].PutValue(40);

                // Ajouter un graphique en secteurs
                int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
                Chart chart = worksheet.Charts[chartIndex];

                // Définir la plage de données du graphique
                chart.NSeries.Add("B2:B5", true);
                chart.NSeries.CategoryData = "A2:A5";

                // Démontrer les différentes valeurs de ChartSplitType
                chart.NSeries[0].SplitType = ChartSplitType.Position;
                Console.WriteLine($"Current SplitType: {chart.NSeries[0].SplitType}");

                // Passer à un autre type de division
                chart.NSeries[0].SplitType = ChartSplitType.PercentValue;
                Console.WriteLine($"Updated SplitType: {chart.NSeries[0].SplitType}");

                // Enregistrez le classeur
                workbook.Save("ChartSplitTypeDemo.xlsx");
                Console.WriteLine("ChartSplitType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ChartSplitType demonstration: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


