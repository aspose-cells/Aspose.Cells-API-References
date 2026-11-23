---
title: "ChartFrame.XRatioToChart"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartFrame. Obtient ou définit la coordonnée x du coin supérieur gauche en unités de ratio de la zone du graphique"
type: docs
url: /fr/net/aspose.cells.charts/chartframe/xratiotochart/
---
## ChartFrame.XRatioToChart property

Obtient ou définit la coordonnée x du coin supérieur gauche en unités du ratio de la zone du graphique.

```csharp
public virtual double XRatioToChart { get; set; }
```

### Remarques

Il s'agit d'une valeur fractionnaire, sa plage valide est comprise entre 0 et 1. Comment convertir les unités de ratio en pixels ? XPixel = XRatioToChart * Chart.ChartObject.Width;

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyXRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accédez au titre du graphique qui est un ChartFrame
            ChartFrame chartTitle = chart.Title;

            // Affichez la valeur actuelle de XRatioToChart
            Console.WriteLine("Current XRatioToChart value: " + chartTitle.XRatioToChart);

            // Définir une nouvelle valeur XRatioToChart (0,5 signifie 50 % de la largeur du graphique depuis la gauche)
            chartTitle.XRatioToChart = 0.5;

            // Afficher la nouvelle position
            Console.WriteLine("Title position after change - XRatioToChart: " + chartTitle.XRatioToChart);

            // Enregistrez le classeur
            workbook.Save("ChartFrameXRatioToChartDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


