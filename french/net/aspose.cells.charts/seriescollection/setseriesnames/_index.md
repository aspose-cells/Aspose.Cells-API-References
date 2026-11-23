---
title: "SeriesCollection.SetSeriesNames"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SeriesCollection. Définit les noms de toutes les séries dans le graphique"
type: docs
url: /fr/net/aspose.cells.charts/seriescollection/setseriesnames/
---
## SeriesCollection.SetSeriesNames method

Définit les noms de toutes les séries du graphique.

```csharp
public void SetSeriesNames(int startIndex, string area, bool isVertical)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startIndex | Int32 | L'index de la première série dont vous souhaitez définir le nom. |
| zone | String | Spécifie la zone pour le nom de la série. |
| isVertical | Boolean | &gt;Spécifie si la série doit être tracée à partir d'une plage de valeurs de cellules par ligne ou par colonne. |

### Remarques

Si l'index de départ est supérieur au nombre de séries, la fonction retournera et ne fera rien. Si vous définissez des données sur des cellules contiguës, utilisez deux‑points pour les séparer. Par exemple, $C$2:$C$5. Si vous définissez des données sur des cellules contiguës, utilisez une virgule pour les séparer. Par exemple, ($C$2,$D$5).

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesCollectionMethodSetSeriesNamesWithInt32StringBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Q1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["C1"].PutValue("Q2");
            worksheet.Cells["C2"].PutValue(120);
            worksheet.Cells["C3"].PutValue(180);
            worksheet.Cells["C4"].PutValue(220);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Obtenir la collection de séries du graphique
            SeriesCollection seriesCollection = chart.NSeries;

            try
            {
                // Appelez SetSeriesNames avec les paramètres (startIndex : 0, area : "A2:A4", isVertical : true)
                seriesCollection.SetSeriesNames(0, "A2:A4", true);

                // Ajouter des données de série
                seriesCollection.Add("B2:C4", true);

                Console.WriteLine("SetSeriesNames method executed successfully with parameters (Int32, String, Boolean)");
                Console.WriteLine("Series names set from range A2:A4");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetSeriesNames method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("SeriesCollectionMethodSetSeriesNamesWithInt32StringBooleanDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


