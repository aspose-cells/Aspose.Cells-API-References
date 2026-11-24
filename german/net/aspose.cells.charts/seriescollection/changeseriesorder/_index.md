---
title: "SeriesCollection.ChangeSeriesOrder"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SeriesCollection Methode. Ändert direkt die Reihenfolge der beiden Serien"
type: docs
url: /de/net/aspose.cells.charts/seriescollection/changeseriesorder/
---
## SeriesCollection.ChangeSeriesOrder method

Ändert direkt die Reihenfolge der beiden Serien.

```csharp
[Obsolete("Use SeriesCollection.SwapSeries property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ChangeSeriesOrder(int sourceIndex, int destIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceIndex | Int32 | Der aktuelle Index |
| destIndex | Int32 | Der Zielindex |

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die SeriesCollection.SwapSeries Methode. Diese Methode wird 12 Monate später, seit Juni 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Diagramm hinzufügen
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

            // Ein Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Serie zum Diagramm hinzufügen
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.Add("C2:C4", true);
            
            // Abrufen der Seriensammlung
            SeriesCollection seriesCollection = chart.NSeries;

            try
            {
                // Rufen Sie die ChangeSeriesOrder-Methode auf, um Serien am Index 0 und 2 zu vertauschen
                seriesCollection.ChangeSeriesOrder(0, 2);
                
                Console.WriteLine("Series order changed successfully. Series at index 0 and 2 swapped.");
                
                // Zeigen Sie die neue Serienreihenfolge an
                for (int i = 0; i < seriesCollection.Count; i++)
                {
                    Console.WriteLine($"Series {i + 1}: {seriesCollection[i].Name}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ChangeSeriesOrder method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("ChangeSeriesOrderWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


