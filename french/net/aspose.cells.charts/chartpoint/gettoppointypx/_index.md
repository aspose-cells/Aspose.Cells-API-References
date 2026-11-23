---
title: "ChartPoint.GetTopPointYPx"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ChartPoint. Obtient la coordonnée y du point supérieur de la forme après l'appel de la méthode Chart.Calculate. S'applique aux graphiques 3D Column3D Bar3D Cone Cylinder Pyramid et Area3D"
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/gettoppointypx/
---
## ChartPoint.GetTopPointYPx method

Obtient la coordonnée y du point supérieur de la forme après avoir appelé la méthode Chart.Calculate(). S'applique aux graphiques 3D : Column3D, Bar3D, Cone, Cylinder, Pyramid et Area3D.

```csharp
public float GetTopPointYPx(int index)
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetTopPointYPxWithInt32Demo
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
            
            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Calculer le graphique pour s'assurer que toutes les propriétés de position sont calculées
            chart.Calculate();
            
            // Obtenir le premier point du graphique de la première série
            ChartPoint point = chart.NSeries[0].Points[0];
            
            try
            {
                // Obtenez le nombre de points supérieurs
                int topPointCount = point.GetTopPointCount();
                
                if (topPointCount > 0)
                {
                    // Appelez GetTopPointYPx avec l'index 0
                    float yPx = point.GetTopPointYPx(0);
                    
                    Console.WriteLine($"Top point Y position in pixels: {yPx}");
                    Console.WriteLine("Method executed successfully with parameter (Int32)");
                }
                else
                {
                    Console.WriteLine("No top points available for this chart point");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTopPointYPx method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("ChartPointMethodGetTopPointYPxWithInt32Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


