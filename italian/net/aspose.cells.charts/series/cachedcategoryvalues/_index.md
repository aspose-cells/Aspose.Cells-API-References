---
title: "Series.CachedCategoryValues"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Ottiene i valori di categoria memorizzati nella cache per la serie"
type: docs
url: /it/net/aspose.cells.charts/series/cachedcategoryvalues/
---
## Series.CachedCategoryValues property

Ottiene i valori di categoria memorizzati nella cache per la serie

```csharp
[Obsolete("internal use only")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList CachedCategoryValues { get; }
```

### Osservazioni

NOTA: Questa proprietà è attualmente destinata solo all'uso interno. Verrà modificata o rimossa nella prossima versione.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(10);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Accedi alla prima serie
                Series series = chart.NSeries[0];

                // Visualizza i valori di categoria memorizzati nella cache
                ArrayList cachedCategoryValues = series.CachedCategoryValues;
                Console.WriteLine("CachedCategoryValues count: " + cachedCategoryValues.Count);

                // Visualizza ogni valore di categoria memorizzato nella cache
                for (int i = 0; i < cachedCategoryValues.Count; i++)
                {
                    Console.WriteLine("Cached Category Value " + (i + 1) + ": " + cachedCategoryValues[i]);
                }

                // Salva la cartella di lavoro
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

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


