---
title: "Walls.GetCubePointYPx"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Walls. Obtient la coordonnée y du point d'extrémité du cube des murs après l'appel de la méthode Chart.Calculate. Le nombre de points d'extrémité du cube des murs est huit"
type: docs
url: /fr/net/aspose.cells.charts/walls/getcubepointypx/
---
## Walls.GetCubePointYPx method

Obtient la coordonnée y du point d'apex du cube des murs après l'appel de la méthode Chart.Calculate(). Le nombre de points d'apex du cube des murs est huit.

```csharp
public float GetCubePointYPx(int index)
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class WallsMethodGetCubePointYPxDemo
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

            // Ajouter un graphique 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculer le graphique pour s'assurer que les propriétés Wall sont renseignées
            chart.Calculate();

            // Obtenir l'objet Walls
            Walls walls = chart.Walls;

            try
            {
                // Obtenir le nombre de points du cube
                int pointCount = walls.GetCubePointCount();

                if (pointCount > 0)
                {
                    // Appeler GetCubePointYPx avec le premier indice (0)
                    float yPx = walls.GetCubePointYPx(0);
                    Console.WriteLine($"Y-coordinate of first cube point in pixels: {yPx}");
                }
                else
                {
                    Console.WriteLine("No cube points available in the walls.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCubePointYPx method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("WallsMethodGetCubePointYPxDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


