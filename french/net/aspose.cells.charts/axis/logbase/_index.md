---
title: "Axis.LogBase"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Axis. Représente la base logarithmique. La valeur par défaut est 10"
type: docs
url: /fr/net/aspose.cells.charts/axis/logbase/
---
## Axis.LogBase property

Représente la base logarithmique. La valeur par défaut est 10.

```csharp
public double LogBase { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyLogBaseDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue(Math.Pow(2, i-2)); // Exponential values
                worksheet.Cells[$"B{i}"].PutValue(i * 10);
            }

            // Créer un graphique
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ajouter une série
            chart.NSeries.Add($"B2:B10", true);
            chart.NSeries[0].XValues = $"A2:A10";
            chart.NSeries[0].Name = "Logarithmic Series";

            // Configurer l'axe logarithmique
            chart.CategoryAxis.IsLogarithmic = true;
            chart.CategoryAxis.LogBase = 2; // Set logarithmic base to 2
            chart.CategoryAxis.Title.Text = "Logarithmic Scale (Base 2)";
            
            // Enregistrez le classeur
            workbook.Save("AxisPropertyLogBaseDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


