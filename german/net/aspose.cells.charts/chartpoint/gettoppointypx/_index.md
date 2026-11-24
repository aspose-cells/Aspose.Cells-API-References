---
title: "ChartPoint.GetTopPointYPx"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Methode. Gibt die y‑Koordinate des oberen Punkts der Form zurück, nachdem die Methode Chart.Calculate aufgerufen wurde. Gilt für 3D‑Diagramme Column3D, Bar3D, Cone, Cylinder, Pyramid und Area3D"
type: docs
url: /de/net/aspose.cells.charts/chartpoint/gettoppointypx/
---
## ChartPoint.GetTopPointYPx method

Ermittelt die y‑Koordinate des oberen Punkts der Form, nachdem die Methode Chart.Calculate() aufgerufen wurde. Gilt für 3D‑Diagramme: Column3D, Bar3D, Cone, Cylinder, Pyramid und Area3D.

```csharp
public float GetTopPointYPx(int index)
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetTopPointYPxWithInt32Demo
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
            
            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Berechne das Diagramm, um sicherzustellen, dass alle Positions-Eigenschaften berechnet werden
            chart.Calculate();
            
            // Hole den ersten Diagrammpunkt aus der ersten Serie
            ChartPoint point = chart.NSeries[0].Points[0];
            
            try
            {
                // Ermitteln Sie die Anzahl der oberen Punkte
                int topPointCount = point.GetTopPointCount();
                
                if (topPointCount > 0)
                {
                    // Rufen Sie GetTopPointYPx mit Index 0 auf
                    float yPx = point.GetTopPointYPx(0);
                    
                    Console.WriteLine($"Top point Y position in pixels: {yPx}");
                    Console.WriteLine("Method executed successfully with parameter (Int32)");
                }
                else
                {
                    Console.WriteLine("No top points available for this chart point");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTopPointYPx method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("ChartPointMethodGetTopPointYPxWithInt32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


