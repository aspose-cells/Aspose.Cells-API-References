---
title: "ChartPoint.ShapeHeightPx"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartPoint. Obtient la hauteur en pixels après l'appel de la méthode Chart.Calculate"
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/shapeheightpx/
---
## ChartPoint.ShapeHeightPx property

Obtient la hauteur en unités de pixels après les appels à la méthode Chart.Calculate().

```csharp
public int ShapeHeightPx { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeHeightPxDemo
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

            // Ajouter un graphique en colonnes
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculez le graphique pour obtenir les dimensions de la forme
            chart.Calculate();

            // Obtenir le premier point du graphique de la première série
            ChartPoint chartPoint = chart.NSeries[0].Points[0];

            // Affichez la hauteur actuelle de la forme du point du graphique en pixels
            Console.WriteLine("Current ShapeHeightPx value: " + chartPoint.ShapeHeightPx);

            // Remarque : ShapeHeightPx est en lecture seule, nous ne pouvons donc pas le définir directement
            // Pour modifier la hauteur, nous devrions modifier la taille du graphique ou les valeurs de données
            // et recalculer le graphique

            // Modifiez la valeur de données qui affectera la taille du point du graphique
            worksheet.Cells["B2"].PutValue(50);
            chart.Calculate();

            // Affichez la nouvelle hauteur après modification des données
            Console.WriteLine("New ShapeHeightPx value after data change: " + chartPoint.ShapeHeightPx);

            // Enregistrez le classeur
            workbook.Save("ChartPointShapeHeightPxDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


