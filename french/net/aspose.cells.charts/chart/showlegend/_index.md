---
title: "Chart.ShowLegend"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Chart. Obtient ou définit une valeur indiquant si la légende du graphique sera affichée. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells.charts/chart/showlegend/
---
## Chart.ShowLegend property

Obtient ou définit une valeur indiquant si la légende du graphique sera affichée. La valeur par défaut est vraie.

```csharp
public bool ShowLegend { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyShowLegendDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B1"].PutValue("Quantity");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Afficher la légende par défaut (true)
            Console.WriteLine("Legend initially visible: " + chart.ShowLegend);
            
            // Masquer la légende
            chart.ShowLegend = false;
            Console.WriteLine("Legend after setting to false: " + chart.ShowLegend);
            
            // Enregistrez le classeur
            workbook.Save("ChartLegendExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


