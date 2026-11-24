---
title: "SeriesCollection.GetSeriesByOrder"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SeriesCollection-Methode. Gibt das Series-Element nach Reihenfolge zurück"
type: docs
url: /de/net/aspose.cells.charts/seriescollection/getseriesbyorder/
---
## SeriesCollection.GetSeriesByOrder method

Gibt das [`Series`](../../series/) Element nach Reihenfolge zurück.

```csharp
public Series GetSeriesByOrder(int order)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Reihenfolge | Int32 | Die Reihenfolge der Serien |

### Rückgabewert

Das Serien-Element

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesCollectionMethodGetSeriesByOrderWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");
            
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["B5"].PutValue(400);
            
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["C4"].PutValue(350);
            worksheet.Cells["C5"].PutValue(450);

            // Ein Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.Add("C2:C5", true);
            chart.NSeries.CategoryData = "A2:A5";

            try
            {
                // Abrufen der ersten Serie (order = 0)
                Series series = chart.NSeries.GetSeriesByOrder(0);
                
                if (series != null)
                {
                    // Ändern Sie die Eigenschaften der Serie
                    series.Name = "Modified Series 1";
                    series.Shadow = true;
                    
                    Console.WriteLine("Successfully retrieved and modified series with order 0");
                    Console.WriteLine($"Series Name: {series.Name}");
                    Console.WriteLine($"Shadow Enabled: {series.Shadow}");
                }
                
                // Speichere die Arbeitsmappe
                workbook.Save("SeriesCollectionMethodGetSeriesByOrderDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSeriesByOrder method: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Series](../../series/)
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


