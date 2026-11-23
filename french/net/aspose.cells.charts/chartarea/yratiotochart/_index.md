---
title: "ChartArea.YRatioToChart"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartArea. Obtient ou obtient le décalage vertical de la ligne de son coin supérieur gauche en unités de ratio de la zone du graphique"
type: docs
url: /fr/net/aspose.cells.charts/chartarea/yratiotochart/
---
## ChartArea.YRatioToChart property

Obtient ou obtient le décalage vertical depuis la ligne du coin supérieur gauche, en unités de proportion de la zone de graphique.

```csharp
public override double YRatioToChart { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartAreaPropertyYRatioToChartDemo
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

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accéder à la zone du graphique
            ChartArea chartArea = chart.ChartArea;

            // Afficher la valeur actuelle de YRatioToChart
            Console.WriteLine("Current YRatioToChart value: " + chartArea.YRatioToChart);

            // Modifier la propriété YRatioToChart (0,0 à 1,0 représente 0 % à 100 % de la zone du graphique)
            chartArea.YRatioToChart = 0.2; // Move chart area down by 20% of chart height

            // Afficher la nouvelle valeur de YRatioToChart
            Console.WriteLine("New YRatioToChart value: " + chartArea.YRatioToChart);

            // Enregistrer le classeur pour voir l'effet
            workbook.Save("ChartAreaPropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


