---
title: "ChartFrame.DefaultYRatioToChart"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartFrame. Représente y de la position par défaut en unités de la fraction de la zone du graphique"
type: docs
url: /fr/net/aspose.cells.charts/chartframe/defaultyratiotochart/
---
## ChartFrame.DefaultYRatioToChart property

Représente le y de la position par défaut en unités de la fraction de la zone du graphique.

```csharp
public double DefaultYRatioToChart { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultYRatioToChartDemo
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
            
            // Ajoutez un graphique et récupérez son cadre de graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);
            
            // Obtenez le cadre du graphique (titre dans ce cas)
            ChartFrame chartFrame = chart.Title;
            
            // Affichez la valeur actuelle de DefaultYRatioToChart
            Console.WriteLine("Current DefaultYRatioToChart value: " + chartFrame.DefaultYRatioToChart);
            
            // Démontrez comment la modification de YRatioToChart affecte la position (puisque DefaultYRatioToChart est en lecture seule)
            Console.WriteLine("Current YRatioToChart value: " + chartFrame.YRatioToChart);
            chartFrame.YRatioToChart = 0.1; // Move title up
            Console.WriteLine("New YRatioToChart value: " + chartFrame.YRatioToChart);
            
            // Enregistrer le résultat
            workbook.Save("PropertyDefaultYRatioToChartDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


