---
title: "ChartPoint.ShapeHeight"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartPoint. Obtient la hauteur en unités de 1/4000 de la hauteur du graphique après l'appel de la méthode Chart.Calculate"
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/shapeheight/
---
## ChartPoint.ShapeHeight property

Obtient la hauteur en unités de 1/4000 de la hauteur du graphique après les appels à la méthode Chart.Calculate().

```csharp
public int ShapeHeight { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeHeightDemo
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
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculer le graphique pour garantir que les propriétés de forme sont disponibles
            chart.Calculate();

            // Obtenir le premier point de la première série
            ChartPoint point = chart.NSeries[0].Points[0];

            // Afficher la valeur actuelle de ShapeHeight (en 1/4000 de la hauteur du graphique)
            Console.WriteLine("Current ShapeHeight value: " + point.ShapeHeight);

            // Remarque : ShapeHeight est en lecture seule, nous ne pouvons donc pas le définir directement
            // Pour modifier la hauteur, nous devons ajuster la taille du graphique ou d'autres propriétés

            // Démontrer l'effet en modifiant la hauteur du graphique
            Console.WriteLine("Original chart height: " + chart.ChartObject.Height);
            chart.ChartObject.Height = 400;
            chart.Calculate(); // Recalculate to update shape properties

            // Afficher la nouvelle valeur de ShapeHeight après avoir modifié la hauteur du graphique
            Console.WriteLine("New ShapeHeight value after chart resize: " + point.ShapeHeight);

            // Enregistrer le résultat
            workbook.Save("ChartPointPropertyShapeHeightDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


