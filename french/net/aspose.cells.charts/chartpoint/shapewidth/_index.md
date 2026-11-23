---
title: "ChartPoint.ShapeWidth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartPoint. Obtient la largeur en unités de 1/4000 de la largeur du graphique après l'appel de la méthode Chart.Calculate"
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/shapewidth/
---
## ChartPoint.ShapeWidth property

Obtient la largeur en unités de 1/4000 de la largeur du graphique après l'appel de la méthode Chart.Calculate().

```csharp
public int ShapeWidth { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeWidthDemo
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
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Calculer le graphique pour garantir que les propriétés de forme sont disponibles
            chart.Calculate();
            
            // Obtenir le premier point du graphique dans la première série
            ChartPoint point = chart.NSeries[0].Points[0];
            
            // Affichez la valeur actuelle de ShapeWidth (en 1/4000 de la largeur du graphique)
            Console.WriteLine("Current ShapeWidth value: " + point.ShapeWidth);
            
            // Affichez la largeur en pixels
            Console.WriteLine("Shape width in pixels: " + point.ShapeWidthPx);
            
            // Remarque : ShapeWidth est en lecture seule, nous ne pouvons donc pas le définir directement
            // Pour modifier la largeur, nous devrions modifier la taille du graphique ou d'autres propriétés
            
            // Enregistrer le résultat
            workbook.Save("ChartPointShapeWidthDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


