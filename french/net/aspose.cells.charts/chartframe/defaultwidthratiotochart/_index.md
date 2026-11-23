---
title: "ChartFrame.DefaultWidthRatioToChart"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartFrame. Représente la largeur de la position par défaut en unités de Fraction de la zone du graphique"
type: docs
url: /fr/net/aspose.cells.charts/chartframe/defaultwidthratiotochart/
---
## ChartFrame.DefaultWidthRatioToChart property

Représente la largeur de la position par défaut en unités de fraction de la zone du graphique.

```csharp
public double DefaultWidthRatioToChart { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultWidthRatioToChartDemo
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

            // Accéder au titre du graphique qui est un ChartFrame
            ChartFrame chartTitle = chart.Title;

            // Afficher la valeur actuelle de DefaultWidthRatioToChart
            Console.WriteLine("Current DefaultWidthRatioToChart value: " + chartTitle.DefaultWidthRatioToChart);

            // Note : DefaultWidthRatioToChart est en lecture seule, donc nous ne pouvons pas le définir
            // À la place, nous démontrerons sa relation avec le ratio de largeur réel
            Console.WriteLine("Current WidthRatioToChart: " + chartTitle.WidthRatioToChart);

            // Modifiez le ratio de largeur pour démontrer son effet
            chartTitle.WidthRatioToChart = 0.5;
            Console.WriteLine("After setting WidthRatioToChart to 0.5, DefaultWidthRatioToChart remains: " + chartTitle.DefaultWidthRatioToChart);

            // Enregistrez le classeur
            workbook.Save("ChartFramePropertyDefaultWidthRatioToChartDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


