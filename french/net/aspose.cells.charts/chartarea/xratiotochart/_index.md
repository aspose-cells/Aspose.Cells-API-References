---
title: "ChartArea.XRatioToChart"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartArea. Obtient ou définit le décalage horizontal depuis la colonne du coin supérieur gauche comme un ratio de la zone du graphique"
type: docs
url: /fr/net/aspose.cells.charts/chartarea/xratiotochart/
---
## ChartArea.XRatioToChart property

Obtient ou définit le décalage horizontal depuis la colonne du coin supérieur gauche, en tant que proportion de la zone de graphique.

```csharp
public override double XRatioToChart { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartAreaPropertyXRatioToChartDemo
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
            chart.SetChartDataRange("A1:B4", true);

            // Obtenez la zone du graphique
            ChartArea chartArea = chart.ChartArea;

            // Affichez la valeur actuelle de XRatioToChart
            Console.WriteLine("Current XRatioToChart value: " + chartArea.XRatioToChart);

            // Modifiez la valeur de XRatioToChart pour déplacer la zone du graphique horizontalement
            chartArea.XRatioToChart = 0.2; // 20% from the left of the chart container

            // Affichez la nouvelle valeur de XRatioToChart
            Console.WriteLine("New XRatioToChart value: " + chartArea.XRatioToChart);

            // Enregistrez le classeur
            workbook.Save("ChartAreaXRatioToChartDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


