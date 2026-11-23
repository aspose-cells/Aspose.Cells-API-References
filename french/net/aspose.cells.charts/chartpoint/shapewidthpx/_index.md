---
title: "ChartPoint.ShapeWidthPx"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartPoint. Obtient la largeur en unités de pixels après l'appel de la méthode Chart.Calculate"
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/shapewidthpx/
---
## ChartPoint.ShapeWidthPx property

Obtient la largeur en unités de pixels après l'appel de la méthode Chart.Calculate().

```csharp
public int ShapeWidthPx { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeWidthPxDemo
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

            // Calculer le graphique pour garantir que les propriétés de forme sont disponibles
            chart.Calculate();

            // Obtenir le premier point du graphique de la première série
            ChartPoint point = chart.NSeries[0].Points[0];

            // Afficher la largeur actuelle de la forme du point du diagramme en pixels
            Console.WriteLine("Current ShapeWidthPx value: " + point.ShapeWidthPx);

            // Remarque : ShapeWidthPx est en lecture seule, nous ne pouvons donc pas le définir directement
            // Pour modifier la largeur, nous devons ajuster la taille du diagramme ou d'autres propriétés
            // cela affecterait la largeur du point lors du prochain Calculate()

            // Modifier la largeur du diagramme pour démontrer comment cela affecte ShapeWidthPx
            chart.ChartObject.Width = 1000;
            chart.Calculate();

            // Afficher la nouvelle largeur après le redimensionnement du diagramme
            Console.WriteLine("New ShapeWidthPx value after chart resize: " + point.ShapeWidthPx);

            // Enregistrer le résultat
            workbook.Save("ChartPointPropertyShapeWidthPxDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


