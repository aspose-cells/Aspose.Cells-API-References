---
title: "Axis.BaseUnitScale"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Axis. Représente l'échelle de l'unité de base pour l'axe des catégories"
type: docs
url: /fr/net/aspose.cells.charts/axis/baseunitscale/
---
## Axis.BaseUnitScale property

Représente l'échelle de l'unité de base pour l'axe de catégorie.

```csharp
public TimeUnit BaseUnitScale { get; set; }
```

### Remarques

Ne prend effet que lorsque la propriété CategoryType est définie sur TimeScale.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyBaseUnitScaleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells[$"A{i}"].PutValue(DateTime.Now.AddDays(i));
                sheet.Cells[$"B{i}"].PutValue(i * 100);
            }

            // Ajoutez un graphique
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Définir l'échelle de l'unité de base pour l'axe des catégories
            chart.CategoryAxis.BaseUnitScale = TimeUnit.Months;

            // Enregistrez le classeur
            workbook.Save("AxisPropertyBaseUnitScaleDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TimeUnit](../../timeunit/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


