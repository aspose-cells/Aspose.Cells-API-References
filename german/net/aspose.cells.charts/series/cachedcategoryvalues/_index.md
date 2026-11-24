---
title: "Series.CachedCategoryValues"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Eigenschaft. Gibt die zwischengespeicherten Kategorienwerte für die Serie zurück"
type: docs
url: /de/net/aspose.cells.charts/series/cachedcategoryvalues/
---
## Series.CachedCategoryValues property

Gibt die zwischengespeicherten Kategorienwerte für die Serie zurück

```csharp
[Obsolete("internal use only")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList CachedCategoryValues { get; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist derzeit nur für den internen Gebrauch vorgesehen. Sie wird in der nächsten Version geändert oder entfernt werden.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Collections;

    public class SeriesPropertyCachedCategoryValuesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(10);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Zugriff auf die erste Serie
                Series series = chart.NSeries[0];

                // Die zwischengespeicherten Kategorienwerte anzeigen
                ArrayList cachedCategoryValues = series.CachedCategoryValues;
                Console.WriteLine("CachedCategoryValues count: " + cachedCategoryValues.Count);

                // Jeden zwischengespeicherten Kategorienwert anzeigen
                for (int i = 0; i < cachedCategoryValues.Count; i++)
                {
                    Console.WriteLine("Cached Category Value " + (i + 1) + ": " + cachedCategoryValues[i]);
                }

                // Speichere die Arbeitsmappe
                workbook.Save("CachedCategoryValuesDemo.xlsx");
                Console.WriteLine("CachedCategoryValues demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


