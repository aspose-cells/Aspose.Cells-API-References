---
title: "Title.XRatioToChart"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Title. Obtient ou définit la coordonnée x du coin supérieur gauche en unités de fraction de la zone du graphique. X en pixels  XRatioToChart  Chart.ChartObject.Width"
type: docs
url: /fr/net/aspose.cells.charts/title/xratiotochart/
---
## Title.XRatioToChart property

Obtient ou définit la coordonnée x du coin supérieur gauche en unités de fraction de la zone du graphique. X en pixels = XRatioToChart * Chart.ChartObject.Width;

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

    public class TitlePropertyXRatioToChartDemo
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

            // Définissez la source de données pour le graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtenez le titre du graphique
            chart.Title.Text = "Sample Chart Title";
            Title title = chart.Title;

            // Affichez la valeur actuelle de XRatioToChart
            Console.WriteLine("Current XRatioToChart value: " + title.XRatioToChart);

            // Modifiez la valeur de XRatioToChart pour déplacer le titre horizontalement
            title.XRatioToChart = 0.25; // 25% from the left of the chart area
            Console.WriteLine("New XRatioToChart value: " + title.XRatioToChart);

            // Enregistrez le classeur
            workbook.Save("TitlePropertyXRatioToChartDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


