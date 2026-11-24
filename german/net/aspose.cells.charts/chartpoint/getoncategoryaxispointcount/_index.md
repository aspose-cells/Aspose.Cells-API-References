---
title: "ChartPoint.GetOnCategoryAxisPointCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Methode. Gibt die Anzahl der Punkte auf der Kategorienachse zurück, nachdem die Methode Chart.Calculate aufgerufen wurde. Gilt nur für Flächendiagramme."
type: docs
url: /de/net/aspose.cells.charts/chartpoint/getoncategoryaxispointcount/
---
## ChartPoint.GetOnCategoryAxisPointCount method

Ermittelt die Anzahl der Punkte auf der Kategorienachse, nachdem die Methode Chart.Calculate() aufgerufen wurde. Gilt nur für Flächendiagramme.

```csharp
public int GetOnCategoryAxisPointCount()
```

### Hinweise

Flächen‑2D‑Diagramm liefert 1, Flächen‑3D‑Diagramm liefert 2.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetOnCategoryAxisPointCountDemo
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

            // Füge ein Flächendiagramm hinzu.
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Berechne das Diagramm, um sicherzustellen, dass alle Diagrammpunkte berechnet wurden.
            chart.Calculate();

            try
            {
                // Hole den ersten Diagrammpunkt aus der ersten Serie
                ChartPoint point = chart.NSeries[0].Points[0];
                
                // Rufe die Methode GetOnCategoryAxisPointCount auf.
                int pointCount = point.GetOnCategoryAxisPointCount();
                
                Console.WriteLine($"Number of points on category axis: {pointCount}");
                
                // Zeige die Koordinaten jedes Punktes auf der Kategorienachse an.
                for (int i = 0; i < pointCount; i++)
                {
                    float x = point.GetOnCategoryAxisPointXPx(i);
                    float y = point.GetOnCategoryAxisPointYPx(i);
                    Console.WriteLine($"Point {i}: X={x}, Y={y}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOnCategoryAxisPointCount method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("MethodGetOnCategoryAxisPointCountDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


