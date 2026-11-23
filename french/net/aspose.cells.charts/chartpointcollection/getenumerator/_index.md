---
title: "ChartPointCollection.GetEnumerator"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ChartPointCollection méthode. Retourne un énumérateur pour l'ensemble de ChartPointCollection"
type: docs
url: /fr/net/aspose.cells.charts/chartpointcollection/getenumerator/
---
## ChartPointCollection.GetEnumerator method

Retourne un énumérateur pour l'ensemble de [`ChartPointCollection`](../).

```csharp
public IEnumerator GetEnumerator()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Collections;

    public class ChartPointCollectionMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["A4"].PutValue("Cat3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Obtenir la collection de points de la première série
                ChartPointCollection points = chart.NSeries[0].Points;

                // Appelez la méthode GetEnumerator
                IEnumerator enumerator = points.GetEnumerator();

                Console.WriteLine("Iterating through chart points:");
                while (enumerator.MoveNext())
                {
                    ChartPoint point = (ChartPoint)enumerator.Current;
                    Console.WriteLine($"Point value: {point.YValue}");
                }

                Console.WriteLine("Method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("MethodGetEnumeratorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


