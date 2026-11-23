---
title: "PlotArea.XRatioToChart"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PlotArea. Obtient ou définit la coordonnée x du coin supérieur gauche du cadre englobant du plot area en tant que ratio de la zone du graphique"
type: docs
url: /fr/net/aspose.cells.charts/plotarea/xratiotochart/
---
## PlotArea.XRatioToChart property

Obtient ou définit la coordonnée x du coin supérieur gauche de la boîte englobante de la zone de tracé en tant que ratio de la zone du graphique.

```csharp
public override double XRatioToChart { get; set; }
```

### Remarques

Le cadre englobant de la zone de tracé comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques de graduation. Si la valeur n'est pas créée par MS Excel, veuillez appeler la méthode Chart.Calculate() avant d'appeler cette méthode.

Le **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** et **HeightRatioToChart** de **PlotArea** représente la boîte englobante de la zone de tracé qui comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques. Si vous souhaitez obtenir la taille réelle de la zone de tracé, vous devez appeler les propriétés **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** et **InnerHeightRatioToChart**.

Pour Excel 2007 ou version ultérieure, la valeur par défaut est zéro. Vous devez récupérer la valeur après avoir appelé Chart.Calculate().

XPixel = XRatioToChart * chart.ChartObject.Width. Remarque : lorsque XRatioToChart est défini, la propriété IsInnerMode sera automatiquement définie sur false.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyXRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Obtenir la zone de tracé du graphique
            PlotArea plotArea = chart.PlotArea;

            // Affichez la valeur actuelle de XRatioToChart
            Console.WriteLine("Current XRatioToChart value: " + plotArea.XRatioToChart);

            // Modifiez la valeur XRatioToChart pour déplacer la zone de tracé horizontalement
            plotArea.XRatioToChart = 0.2; // 20% from the left of the chart area

            // Affichez la nouvelle valeur de XRatioToChart
            Console.WriteLine("New XRatioToChart value: " + plotArea.XRatioToChart);

            // Enregistrer le classeur pour voir l'effet
            workbook.Save("PlotAreaXRatioToChartDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


