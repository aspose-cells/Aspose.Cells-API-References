---
title: "ChartPoint.GetOnCategoryAxisPointYPx"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ChartPoint. Obtient la coordonnée y du point sur l'axe des catégories après l'appel de la méthode Chart.Calculate. S'applique uniquement au graphique en aires"
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/getoncategoryaxispointypx/
---
## ChartPoint.GetOnCategoryAxisPointYPx method

Obtient la coordonnée y du point sur l'axe des catégories après avoir appelé la méthode Chart.Calculate(). S'applique uniquement aux graphiques de type Area.

```csharp
public float GetOnCategoryAxisPointYPx(int index)
```

### Remarques

Graphique de zone 2D : l'index est 0. Graphique de zone 3D : l'index est 0 ou 1.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetOnCategoryAxisPointYPxWithInt32Demo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 20, 10);
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
                // Appeler GetOnCategoryAxisPointYPx avec l'index 0
                float yPx = point.GetOnCategoryAxisPointYPx(0);
                
                // Afficher le résultat
                Console.WriteLine($"Y coordinate of point on category axis: {yPx} pixels");
                
                // Enregistrez le classeur
                workbook.Save("ChartPointGetOnCategoryAxisPointYPxDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOnCategoryAxisPointYPx method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


