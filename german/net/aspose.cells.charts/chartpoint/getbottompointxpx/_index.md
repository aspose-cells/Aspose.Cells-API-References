---
title: "ChartPoint.GetBottomPointXPx"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Methode. Gibt die x‑Koordinate des unteren Punktes der Form nach Aufruf der Chart.Calculate‑Methode zurück. Gilt für 3D‑Diagramme Column3D, Bar3D, Cone, Cylinder, Pyramid."
type: docs
url: /de/net/aspose.cells.charts/chartpoint/getbottompointxpx/
---
## ChartPoint.GetBottomPointXPx method

Ermittelt die x‑Koordinate des unteren Punkts der Form, nachdem die Methode Chart.Calculate() aufgerufen wurde. Gilt für 3D‑Diagramme: Column3D, Bar3D, Cone, Cylinder, Pyramid.

```csharp
public float GetBottomPointXPx(int index)
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetBottomPointXPxWithInt32Demo
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
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Berechne das Diagramm, um sicherzustellen, dass alle Positions‑Eigenschaften gesetzt sind.
            chart.Calculate();

            try
            {
                // Hole den ersten Diagrammpunkt aus der ersten Serie
                ChartPoint point = chart.NSeries[0].Points[0];

                // Anzahl der unteren Punkte abrufen
                int bottomPointCount = point.GetBottomPointCount();

                if (bottomPointCount > 0)
                {
                    // Rufe GetBottomPointXPx mit Index 0 auf.
                    float xPos = point.GetBottomPointXPx(0);
                    Console.WriteLine($"X position of bottom point (pixels): {xPos}");
                }
                else
                {
                    Console.WriteLine("No bottom points available for this chart point");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBottomPointXPx method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("ChartPointMethodGetBottomPointXPxWithInt32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


