---
title: "Chart.AutoScaling"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Chart. Vrai si Microsoft Excel met à l’échelle un graphique 3D afin qu’il soit plus proche en taille du graphique 2D équivalent. La propriété RightAngleAxes doit être vraie."
type: docs
url: /fr/net/aspose.cells.charts/chart/autoscaling/
---
## Chart.AutoScaling property

Vrai si Microsoft Excel met à l'échelle un graphique 3D de manière à ce qu'il soit plus proche en taille du graphique 2D équivalent. La propriété RightAngleAxes doit être vraie.

```csharp
public bool AutoScaling { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyAutoScalingDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Démontrer la propriété AutoScaling
            chart.AutoScaling = false;
            Console.WriteLine("Chart AutoScaling is set to: " + chart.AutoScaling);

            // Enregistrez le classeur
            workbook.Save("ChartAutoScalingDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


