---
title: "Title.YRatioToChart"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Title. Obtient ou définit la coordonnée y du coin supérieur gauche en unités de fraction de la zone du graphique. Y en pixels  YRatioToChart  Chart.ChartObject.Width"
type: docs
url: /fr/net/aspose.cells.charts/title/yratiotochart/
---
## Title.YRatioToChart property

Obtient ou définit la coordonnée y du coin supérieur gauche en unités de fraction de la zone du graphique. Y en pixels = YRatioToChart * Chart.ChartObject.Width;

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

    public class TitlePropertyYRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtenez le titre du graphique
            chart.Title.Text = "Sample Chart Title";
            Title chartTitle = chart.Title;

            // Afficher la valeur actuelle de YRatioToChart
            Console.WriteLine("Current YRatioToChart value: " + chartTitle.YRatioToChart);

            // Modifier la propriété YRatioToChart pour déplacer le titre verticalement
            chartTitle.YRatioToChart = 0.1; // 10% from the top of the chart area
            Console.WriteLine("New YRatioToChart value: " + chartTitle.YRatioToChart);

            // Enregistrez le classeur
            workbook.Save("TitlePropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


