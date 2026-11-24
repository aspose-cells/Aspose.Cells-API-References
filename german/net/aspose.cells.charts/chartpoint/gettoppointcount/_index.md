---
title: "ChartPoint.GetTopPointCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Methode. Gibt die Anzahl der oberen Punkte zurück, nachdem die Methode Chart.Calculate aufgerufen wurde"
type: docs
url: /de/net/aspose.cells.charts/chartpoint/gettoppointcount/
---
## ChartPoint.GetTopPointCount method

Ermittelt die Anzahl der oberen Punkte, nachdem die Methode Chart.Calculate() aufgerufen wurde.

```csharp
public int GetTopPointCount()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetTopPointCountDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ein Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Berechnen Sie das Diagramm, um sicherzustellen, dass alle Eigenschaften gesetzt sind
            chart.Calculate();

            try
            {
                // Den ersten Punkt in der ersten Serie abrufen
                ChartPoint point = chart.NSeries[0].Points[0];
                
                // Rufen Sie die Methode GetTopPointCount auf
                int topPointCount = point.GetTopPointCount();
                
                // Ergebnis anzeigen
                Console.WriteLine($"Number of top points: {topPointCount}");
                
                // Demonstrieren Sie das Abrufen der Koordinaten des oberen Punktes
                if (topPointCount > 0)
                {
                    for (int i = 0; i < topPointCount; i++)
                    {
                        float x = point.GetTopPointXPx(i);
                        float y = point.GetTopPointYPx(i);
                        Console.WriteLine($"Top point {i + 1} coordinates: ({x}, {y})");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTopPointCount method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("MethodGetTopPointCountDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


