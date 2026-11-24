---
title: "Series.CachedValues"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series‑Eigenschaft. Liefert die zwischengespeicherten Werte für die Serie"
type: docs
url: /de/net/aspose.cells.charts/series/cachedvalues/
---
## Series.CachedValues property

Liefert die zwischengespeicherten Werte für die Serie

```csharp
[Obsolete("internal use only")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList CachedValues { get; }
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

    public class SeriesPropertyCachedValuesDemo
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

                // Zeige die zwischengespeicherten Werte an
                ArrayList cachedValues = series.CachedValues;
                Console.WriteLine("CachedValues count: " + cachedValues.Count);

                // Zeige jeden zwischengespeicherten Wert an
                for (int i = 0; i < cachedValues.Count; i++)
                {
                    Console.WriteLine("Cached Value " + (i + 1) + ": " + cachedValues[i]);
                }

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


