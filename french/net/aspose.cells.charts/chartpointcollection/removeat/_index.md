---
title: "ChartPointCollection.RemoveAt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ChartPointCollection. Supprime le point à l'index de la série"
type: docs
url: /fr/net/aspose.cells.charts/chartpointcollection/removeat/
---
## ChartPointCollection.RemoveAt method

Supprime le point à l'index de la série.

```csharp
public void RemoveAt(int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | L'index du point. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointCollectionMethodRemoveAtWithInt32Demo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtenir la collection de points de la première série
            ChartPointCollection points = chart.NSeries[0].Points;

            try
            {
                // Afficher le nombre initial
                Console.WriteLine($"Initial points count: {points.Count}");

                // Supprimer le point à l'index 1 (deuxième point)
                points.RemoveAt(1);

                // Afficher le résultat
                Console.WriteLine($"Points count after RemoveAt: {points.Count}");
                Console.WriteLine("Point at index 1 removed successfully.");

                // Enregistrez le classeur
                workbook.Save("ChartPointCollectionRemoveAtDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


