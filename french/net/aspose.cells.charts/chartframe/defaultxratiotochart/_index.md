---
title: "ChartFrame.DefaultXRatioToChart"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartFrame. Représente x de la position par défaut en unités de Fraction de la zone du graphique"
type: docs
url: /fr/net/aspose.cells.charts/chartframe/defaultxratiotochart/
---
## ChartFrame.DefaultXRatioToChart property

Représente x de la position par défaut en unités de fraction de la zone du graphique.

```csharp
public double DefaultXRatioToChart { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultXRatioToChartDemo
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

            // Obtenir le cadre du titre du graphique
            ChartFrame titleFrame = chart.Title;

            // Afficher la valeur actuelle de DefaultXRatioToChart
            Console.WriteLine("Default X Ratio To Chart (Title): " + titleFrame.DefaultXRatioToChart);

            // Créer une zone de texte dans le graphique
            Aspose.Cells.Drawing.TextBox textBox = chart.Shapes.AddTextBoxInChart(50, 50, 200, 100);
            
            // Obtenir les propriétés de forme de la zone de texte au lieu d'essayer d'accéder directement à ChartFrame
            Console.WriteLine("Default X Ratio To Chart (TextBox): " + titleFrame.DefaultXRatioToChart);

            // Démontrer comment ces ratios par défaut affectent le positionnement
            Console.WriteLine("Title X Position (Ratio): " + titleFrame.XRatioToChart);
            Console.WriteLine("TextBox X Position (Ratio): " + titleFrame.XRatioToChart);

            // Enregistrez le classeur
            workbook.Save("ChartFrameDefaultXRatioToChartDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


