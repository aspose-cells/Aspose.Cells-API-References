---
title: "SeriesCollection.SwapSeries"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SeriesCollection-metoden. Ändrar direkt ordningen för de två serierna"
type: docs
url: /sv/net/aspose.cells.charts/seriescollection/swapseries/
---
## SeriesCollection.SwapSeries method

Ändrar direkt ordningen för de två serierna.

```csharp
public void SwapSeries(int sourceIndex, int destIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceIndex | Int32 | Det aktuella indexet |
| destIndex | Int32 | Det dest-indexet |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
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

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("A1:C4", true);
            
            // Hämta seriekollektionen
            Aspose.Cells.Charts.SeriesCollection sc = chart.NSeries;
            
            // Skriv ut ursprungliga serienamn
            Console.WriteLine("Original Series Order:");
            for (int i = 0; i < sc.Count; i++)
            {
                Console.WriteLine($"Series {i}: {sc[i].Name}");
            }
            
            // Byt plats på serierna 0 och 1
            sc.SwapSeries(0, 1);
            Console.WriteLine("\nAfter swapping series 0 and 1:");
            for (int i = 0; i < sc.Count; i++)
            {
                Console.WriteLine($"Series {i}: {sc[i].Name}");
            }
            
            // Byt plats på serierna 2 och 0
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

### Se även

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


