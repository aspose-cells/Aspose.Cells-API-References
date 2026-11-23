---
title: "Axis.IsVisible"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Axis. Indique si l'axe est visible"
type: docs
url: /fr/net/aspose.cells.charts/axis/isvisible/
---
## Axis.IsVisible property

Représente si l'axe est visible.

```csharp
public bool IsVisible { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ajouter une série d'axe secondaire
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries[1].PlotOnSecondAxis = true;

            // Démontrer la propriété IsVisible
            Console.WriteLine("Secondary Value Axis Visible: " + chart.SecondValueAxis.IsVisible);
            
            // Masquer l'axe secondaire
            chart.SecondValueAxis.IsVisible = false;
            Console.WriteLine("After setting to false - Secondary Value Axis Visible: " + chart.SecondValueAxis.IsVisible);

            // Enregistrez le classeur
            workbook.Save("AxisIsVisibleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


