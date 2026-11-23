---
title: "ChartPoint.GetTopPointCount"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ChartPoint. Obtient le nombre de points supérieurs après l'appel de la méthode Chart.Calculate"
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/gettoppointcount/
---
## ChartPoint.GetTopPointCount method

Obtient le nombre de points supérieurs après avoir appelé la méthode Chart.Calculate().

```csharp
public int GetTopPointCount()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetTopPointCountDemo
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

            // Calculez le graphique pour vous assurer que toutes les propriétés sont définies
            chart.Calculate();

            try
            {
                // Obtenir le premier point de la première série
                ChartPoint point = chart.NSeries[0].Points[0];
                
                // Appeler la méthode GetTopPointCount
                int topPointCount = point.GetTopPointCount();
                
                // Afficher le résultat
                Console.WriteLine($"Number of top points: {topPointCount}");
                
                // Démontrer l'obtention des coordonnées du point supérieur
                if (topPointCount > 0)
                {
                    for (int i = 0; i < topPointCount; i++)
                    {
                        float x = point.GetTopPointXPx(i);
                        float y = point.GetTopPointYPx(i);
                        Console.WriteLine($"Top point {i + 1} coordinates: ({x}, {y})");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTopPointCount method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("MethodGetTopPointCountDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


