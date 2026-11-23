---
title: "SeriesCollection.SwapSeries"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SeriesCollection. Modifie directement l'ordre des deux séries"
type: docs
url: /fr/net/aspose.cells.charts/seriescollection/swapseries/
---
## SeriesCollection.SwapSeries method

Modifie directement l'ordre des deux séries.

```csharp
public void SwapSeries(int sourceIndex, int destIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceIndex | Int32 | L'index actuel |
| destIndex | Int32 | L'index de destination |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodSwapSeriesWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            
            worksheet.Cells["B1"].PutValue("Series 2");
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(10);
            worksheet.Cells["B4"].PutValue(15);
            
            worksheet.Cells["C1"].PutValue("Series 3");
            worksheet.Cells["C2"].PutValue(8);
            worksheet.Cells["C3"].PutValue(16);
            worksheet.Cells["C4"].PutValue(24);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("A1:C4", true);
            
            // Obtenir la collection de séries
            Aspose.Cells.Charts.SeriesCollection sc = chart.NSeries;
            
            // Afficher les noms des séries originales
            Console.WriteLine("Original Series Order:");
            for (int i = 0; i < sc.Count; i++)
            {
                Console.WriteLine($"Series {i}: {sc[i].Name}");
            }
            
            // Échanger les séries 0 et 1
            sc.SwapSeries(0, 1);
            Console.WriteLine("\nAfter swapping series 0 and 1:");
            for (int i = 0; i < sc.Count; i++)
            {
                Console.WriteLine($"Series {i}: {sc[i].Name}");
            }
            
            // Échanger les séries 2 et 0
            sc.SwapSeries(2, 0);
            Console.WriteLine("\nAfter swapping series 2 and 0:");
            for (int i = 0; i < sc.Count; i++)
            {
                Console.WriteLine($"Series {i}: {sc[i].Name}");
            }
        }
    }
}
```

### Voir aussi

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


