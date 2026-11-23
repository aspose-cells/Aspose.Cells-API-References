---
title: "ChartShape.Chart"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartShape. Retourne un objet Chart qui représente le graphique contenu dans l'objet"
type: docs
url: /fr/net/aspose.cells.drawing/chartshape/chart/
---
## ChartShape.Chart property

Renvoie un objet Chart qui représente le graphique contenu dans l'objet.

```csharp
public Chart Chart { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ChartShapePropertyChartDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["A4"].PutValue("Grains");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtenir l'instance de ChartShape
            ChartShape chartShape = (ChartShape)chart.ChartObject;

            // Accéder à la propriété Chart (lecture seule)
            Chart accessedChart = chartShape.Chart;

            // Afficher les propriétés du graphique
            Console.WriteLine("Chart Name: " + accessedChart.Name);
            Console.WriteLine("Chart Type: " + accessedChart.Type);
            Console.WriteLine("Show Legend: " + accessedChart.ShowLegend);

            // Modifier les propriétés du graphique via l'objet Chart
            accessedChart.Name = "Sales Chart";
            accessedChart.ShowLegend = false;
            accessedChart.Title.Text = "Product Sales Distribution";

            // Modifier le type de graphique
            accessedChart.Type = ChartType.Pie;

            // Enregistrer le résultat
            workbook.Save("ChartShapePropertyChartDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Chart](../../../aspose.cells.charts/chart/)
* class [ChartShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


