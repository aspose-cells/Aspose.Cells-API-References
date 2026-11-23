---
title: "Series.CachedValues"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Obtient les valeurs mises en cache pour la série"
type: docs
url: /fr/net/aspose.cells.charts/series/cachedvalues/
---
## Series.CachedValues property

Obtient les valeurs mises en cache pour la série

```csharp
[Obsolete("internal use only")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList CachedValues { get; }
```

### Remarques

NOTE : Cette propriété est actuellement réservée à un usage interne uniquement. Elle sera modifiée ou supprimée dans la prochaine version.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Collections;

    public class SeriesPropertyCachedValuesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(10);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Accéder à la première série
                Series series = chart.NSeries[0];

                // Afficher les valeurs mises en cache
                ArrayList cachedValues = series.CachedValues;
                Console.WriteLine("CachedValues count: " + cachedValues.Count);

                // Afficher chaque valeur mise en cache
                for (int i = 0; i < cachedValues.Count; i++)
                {
                    Console.WriteLine("Cached Value " + (i + 1) + ": " + cachedValues[i]);
                }

                // Enregistrez le classeur
                workbook.Save("CachedValuesDemo.xlsx");
                Console.WriteLine("CachedValues demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


