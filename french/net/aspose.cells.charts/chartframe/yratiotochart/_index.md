---
title: "ChartFrame.YRatioToChart"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartFrame. Obtient ou définit la coordonnée y du coin supérieur gauche en unités du ratio de la zone du graphique"
type: docs
url: /fr/net/aspose.cells.charts/chartframe/yratiotochart/
---
## ChartFrame.YRatioToChart property

Obtient ou définit la coordonnée y du coin supérieur gauche en unités du ratio de la zone du graphique.

```csharp
public virtual double YRatioToChart { get; set; }
```

### Remarques

Il s'agit d'une valeur fractionnaire, sa plage valide est comprise entre 0 et 1. Comment convertir les unités de ratio en pixels ? YPixel = YRatioToChart * Chart.ChartObject.Height;

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyYRatioToChartDemo
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
            
            // Accédez au titre du graphique qui hérite de ChartFrame
            chart.Title.Text = "Sample Chart";
            
            // Afficher la valeur actuelle de YRatioToChart
            Console.WriteLine("Current Title YRatioToChart value: " + chart.Title.YRatioToChart);
            
            // Modifier la position Y du titre par rapport à la zone du graphique
            chart.Title.YRatioToChart = 0.1; // 10% from top of chart area
            
            // Afficher la nouvelle valeur YRatioToChart
            Console.WriteLine("New Title YRatioToChart value: " + chart.Title.YRatioToChart);
            
            // Accéder à la légende qui hérite également de ChartFrame
            chart.Legend.Position = LegendPositionType.Top;
            
            // Afficher la valeur actuelle YRatioToChart pour la légende
            Console.WriteLine("Current Legend YRatioToChart value: " + chart.Legend.YRatioToChart);
            
            // Modifier la position Y de la légende par rapport à la zone du graphique
            chart.Legend.YRatioToChart = 0.15; // 15% from top of chart area
            
            // Afficher la nouvelle valeur YRatioToChart pour la légende
            Console.WriteLine("New Legend YRatioToChart value: " + chart.Legend.YRatioToChart);
            
            // Enregistrez le classeur
            workbook.Save("ChartFramePropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


