---
title: "ChartPoint.GetTopPointXPx"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Methode. Gibt die x-Koordinate des oberen Punkts der Form zurück, nachdem die Methode Chart.Calculate aufgerufen wurde. Gilt für 3D-Diagramme Column3D Bar3D Cone Cylinder Pyramid und Area3D"
type: docs
url: /de/net/aspose.cells.charts/chartpoint/gettoppointxpx/
---
## ChartPoint.GetTopPointXPx method

Ermittelt die x‑Koordinate des oberen Punkts der Form, nachdem die Methode Chart.Calculate() aufgerufen wurde. Gilt für 3D‑Diagramme: Column3D, Bar3D, Cone, Cylinder, Pyramid und Area3D.

```csharp
public float GetTopPointXPx(int index)
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetTopPointXPxWithInt32Demo
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
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Berechne das Diagramm, um sicherzustellen, dass alle Positions-Eigenschaften berechnet werden
            chart.Calculate();

            try
            {
                // Hole den ersten Diagrammpunkt aus der ersten Serie
                ChartPoint point = chart.NSeries[0].Points[0];

                // Ermitteln Sie die Anzahl der oberen Punkte
                int pointCount = point.GetTopPointCount();

                if (pointCount > 0)
                {
                    // Rufen Sie GetTopPointXPx mit Index 0 auf
                    float xPos = point.GetTopPointXPx(0);
                    Console.WriteLine($"X position of top point (pixels): {xPos}");
                }
                else
                {
                    Console.WriteLine("No top points available for this chart point");
                }

                Console.WriteLine("Method executed successfully with parameters (Int32)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTopPointXPx method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("ChartPointMethodGetTopPointXPxWithInt32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


