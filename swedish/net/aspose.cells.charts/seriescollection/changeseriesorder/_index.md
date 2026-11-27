---
title: "SeriesCollection.ChangeSeriesOrder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SeriesCollection-metoden. Ändrar direkt ordningen för de två serierna"
type: docs
url: /sv/net/aspose.cells.charts/seriescollection/changeseriesorder/
---
## SeriesCollection.ChangeSeriesOrder method

Ändrar direkt ordningen för de två serierna.

```csharp
[Obsolete("Use SeriesCollection.SwapSeries property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ChangeSeriesOrder(int sourceIndex, int destIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceIndex | Int32 | Det aktuella indexet |
| destIndex | Int32 | Det dest-indexet |

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället SeriesCollection.SwapSeries-metoden. Denna metod kommer att tas bort 12 månader senare sedan juni 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesCollectionMethodChangeSeriesOrderWithInt32Int32Demo
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
            worksheet.Cells["B2"].PutValue(40);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(60);
            
            worksheet.Cells["C1"].PutValue("Series 3");
            worksheet.Cells["C2"].PutValue(70);
            worksheet.Cells["C3"].PutValue(80);
            worksheet.Cells["C4"].PutValue(90);

            // Skapa ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till serier i diagrammet
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.Add("C2:C4", true);
            
            // Hämta seriekollektionen
            SeriesCollection seriesCollection = chart.NSeries;

            try
            {
                // Anropa ChangeSeriesOrder-metoden för att byta plats på serierna på index 0 och 2
                seriesCollection.ChangeSeriesOrder(0, 2);
                
                Console.WriteLine("Series order changed successfully. Series at index 0 and 2 swapped.");
                
                // Visa den nya serieordningen
                for (int i = 0; i < seriesCollection.Count; i++)
                {
                    Console.WriteLine($"Series {i + 1}: {seriesCollection[i].Name}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ChangeSeriesOrder method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("ChangeSeriesOrderWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Se även

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


