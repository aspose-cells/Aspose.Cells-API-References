---
title: "ChartPoint.ShapeYPx"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartPoint. Obtient la coordonnée y du coin supérieur gauche en unités de pixels après l'appel de la méthode Chart.Calculate."
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/shapeypx/
---
## ChartPoint.ShapeYPx property

Obtient la coordonnée y du coin supérieur gauche en unités de pixels après les appels à la méthode Chart.Calculate().

```csharp
public int ShapeYPx { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeYPxDemo
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

            // Calculer le graphique pour obtenir les positions des formes
            chart.Calculate();

            // Obtenir le premier point de la première série
            ChartPoint point = chart.NSeries[0].Points[0];

            // Afficher la position Y actuelle en pixels
            Console.WriteLine("Current ShapeYPx value: " + point.ShapeYPx);

            // Remarque : ShapeYPx est en lecture seule, nous ne pouvons donc pas le définir directement
            // Pour changer la position, nous devons modifier la taille/position du graphique ou les données

            // Démontrer l'effet en modifiant la position du graphique, ce qui affectera les positions des points
            chart.Move(2, 3, 17, 11); // Move chart to row 2, column 3
            chart.Calculate(); // Recalculate to update positions

            // Afficher la nouvelle position Y après le déplacement du graphique
            Console.WriteLine("New ShapeYPx value after chart movement: " + point.ShapeYPx);

            // Enregistrer le résultat
            workbook.Save("ChartPointShapeYPxDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


