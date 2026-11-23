---
title: "PlotArea.InnerHeightRatioToChart"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PlotArea. Obtient ou définit la hauteur de la zone de tracé en unités du ratio de la zone du graphique."
type: docs
url: /fr/net/aspose.cells.charts/plotarea/innerheightratiotochart/
---
## PlotArea.InnerHeightRatioToChart property

Obtient ou définit la hauteur de la zone de tracé en unités du ratio de la zone du graphique.

```csharp
public double InnerHeightRatioToChart { get; set; }
```

### Remarques

Le cadre englobant de la zone de tracé comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques de graduation. Si la valeur n'est pas créée par MS Excel, veuillez appeler la méthode Chart.Calculate() avant d'appeler cette méthode.

Le **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** et **HeightRatioToChart** de **PlotArea** représente la boîte englobante de la zone de tracé qui comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques. Si vous souhaitez obtenir la taille réelle de la zone de tracé, vous devez appeler les propriétés **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** et **InnerHeightRatioToChart**.

Pour Excel 2007 ou version ultérieure, la valeur par défaut est zéro. Vous devez récupérer la valeur après avoir appelé Chart.Calculate().

InnerHeight en pixels = InnerXRatioToChart * chart.ChartObject.Width. Remarque : lorsque InnerHeightRatioToChart est défini, la propriété IsInnerMode sera automatiquement définie sur True.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyInnerHeightRatioToChartDemo
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

            // Accéder à la zone de tracé
            PlotArea plotArea = chart.PlotArea;

            // Afficher la valeur actuelle de InnerHeightRatioToChart
            Console.WriteLine("Current InnerHeightRatioToChart value: " + plotArea.InnerHeightRatioToChart);

            // Définir une nouvelle valeur pour InnerHeightRatioToChart (0,5 = 50 % de la hauteur de la zone du graphique)
            plotArea.InnerHeightRatioToChart = 0.5;

            // Démontrez l'effet en enregistrant le classeur
            workbook.Save("PlotAreaInnerHeightRatioToChartDemo.xlsx");

            // Afficher la nouvelle valeur
            Console.WriteLine("New InnerHeightRatioToChart value: " + plotArea.InnerHeightRatioToChart);
        }
    }
}
```

### Voir aussi

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


