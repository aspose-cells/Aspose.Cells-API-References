---
title: "Walls.GetCubePointCount"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Walls. Obtient le nombre de points du cube après l'appel de la méthode Chart.Calculate"
type: docs
url: /fr/net/aspose.cells.charts/walls/getcubepointcount/
---
## Walls.GetCubePointCount method

Obtient le nombre de points du cube après l'appel de la méthode Chart.Calculate().

```csharp
public int GetCubePointCount()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class WallsMethodGetCubePointCountDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculer le graphique pour s'assurer que les propriétés Wall sont disponibles
            chart.Calculate();

            try
            {
                // Obtenir l'objet Walls
                Walls walls = chart.Walls;
                
                // Appeler la méthode GetCubePointCount
                int pointCount = walls.GetCubePointCount();
                
                // Afficher le résultat
                Console.WriteLine($"Number of cube points in chart walls: {pointCount}");
                
                // Enregistrez le classeur
                workbook.Save("WallsMethodGetCubePointCountDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCubePointCount method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


