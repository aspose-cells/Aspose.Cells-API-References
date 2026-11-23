---
title: "ChartPoint.GetOnCategoryAxisPointXPx"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ChartPoint. Obtient la coordonnée x du point sur l'axe des catégories après l'appel de la méthode Chart.Calculate. S'applique uniquement aux graphiques de type Zone."
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/getoncategoryaxispointxpx/
---
## ChartPoint.GetOnCategoryAxisPointXPx method

Obtient la coordonnée x du point sur l'axe des catégories après les appels à la méthode Chart.Calculate(). S'applique uniquement au graphique en aires.

```csharp
public float GetOnCategoryAxisPointXPx(int index)
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

    public class ChartPointMethodGetOnCategoryAxisPointXPxWithInt32Demo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculer le graphique
            chart.Calculate();

            try
            {
                // Obtenir le premier point du graphique
                ChartPoint point = chart.NSeries[0].Points[0];

                // Appeler GetOnCategoryAxisPointXPx avec l'index 0
                float xPosition = point.GetOnCategoryAxisPointXPx(0);

                // Afficher le résultat
                Console.WriteLine($"X position of first category axis point: {xPosition} pixels");

                // Enregistrez le classeur
                workbook.Save("ChartPointGetOnCategoryAxisPointXPxDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOnCategoryAxisPointXPx method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


