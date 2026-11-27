---
title: "SeriesCollection.SetSeriesNames"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SeriesCollection‑metod. Anger namnen på alla serier i diagrammet"
type: docs
url: /sv/net/aspose.cells.charts/seriescollection/setseriesnames/
---
## SeriesCollection.SetSeriesNames method

Anger namnen på alla serier i diagrammet.

```csharp
public void SetSeriesNames(int startIndex, string area, bool isVertical)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startIndex | Int32 | Indexet för den första serien som du vill ange namn på. |
| område | String | Anger området för seriens namn. |
| ärVertikal | Boolean | &gt;Anger om serien ska plottas från ett område med cellvärden radvis eller kolumnvis. |

### Anmärkningar

Om startindexet är större än antalet serier, återgår den och gör ingenting. Om data sätts på sammanhängande celler, använd kolon för att separera dem. Till exempel $C$2:$C$5. Om data sätts på sammanhängande celler, använd komma för att separera dem. Till exempel ($C$2,$D$5).

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i celler
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

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Hämta diagrammets seriekollektion
            SeriesCollection seriesCollection = chart.NSeries;

            try
            {
                // Anropa SetSeriesNames med parametrarna (startIndex: 0, area: "A2:A4", isVertical: true)
                seriesCollection.SetSeriesNames(0, "A2:A4", true);

                // Lägg till seriedata
                seriesCollection.Add("B2:C4", true);

                Console.WriteLine("SetSeriesNames method executed successfully with parameters (Int32, String, Boolean)");
                Console.WriteLine("Series names set from range A2:A4");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetSeriesNames method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("SeriesCollectionMethodSetSeriesNamesWithInt32StringBooleanDemo.xlsx");
        }
    }
}
```

### Se även

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


