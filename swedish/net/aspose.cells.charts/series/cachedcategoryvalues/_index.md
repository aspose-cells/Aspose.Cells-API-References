---
title: "Series.CachedCategoryValues"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Hämtar de cachade kategorivärdena för serien"
type: docs
url: /sv/net/aspose.cells.charts/series/cachedcategoryvalues/
---
## Series.CachedCategoryValues property

Hämtar de cachade kategorivärdena för serien

```csharp
[Obsolete("internal use only")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList CachedCategoryValues { get; }
```

### Anmärkningar

OBS: Denna egenskap är för närvarande endast för internt bruk. Den kommer att ändras eller tas bort i nästa version.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(10);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Åtkomst till den första serien
                Series series = chart.NSeries[0];

                // Visa de cachade kategorivärdena
                ArrayList cachedCategoryValues = series.CachedCategoryValues;
                Console.WriteLine("CachedCategoryValues count: " + cachedCategoryValues.Count);

                // Visa varje cachat kategorivärde
                for (int i = 0; i < cachedCategoryValues.Count; i++)
                {
                    Console.WriteLine("Cached Category Value " + (i + 1) + ": " + cachedCategoryValues[i]);
                }

                // Spara arbetsboken
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

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


