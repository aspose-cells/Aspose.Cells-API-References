---
title: "Walls.GetCubePointXPx"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Walls. Obtient la coordonnée x du point d'apex du cube des murs après l'appel de la méthode Chart.Calculate. Le nombre de points d'apex du cube des murs est huit"
type: docs
url: /fr/net/aspose.cells.charts/walls/getcubepointxpx/
---
## Walls.GetCubePointXPx method

Obtient la coordonnée x du point d'apex du cube des murs après avoir appelé la méthode Chart.Calculate(). Le nombre de points d'apex du cube des murs est huit.

```csharp
public float GetCubePointXPx(int index)
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class WallsMethodGetCubePointXPxWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);
            worksheet.Cells["B5"].PutValue(4000);

            // Créez un graphique 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Calculer le graphique pour s'assurer que les propriétés Wall sont disponibles
            chart.Calculate();

            // Obtenir l'objet Walls
            Walls walls = chart.Walls;

            try
            {
                // Obtenez le nombre de points du cube
                int pointCount = walls.GetCubePointCount();

                if (pointCount > 0)
                {
                    // Appelez GetCubePointXPx avec l'index 0 (premier point)
                    float xCoordinate = walls.GetCubePointXPx(0);
                    
                    Console.WriteLine($"X coordinate of first cube point in pixels: {xCoordinate}");
                    Console.WriteLine("Method executed successfully with parameter (Int32)");
                }
                else
                {
                    Console.WriteLine("No cube points available in the walls");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCubePointXPx method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("WallsMethodGetCubePointXPxDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


