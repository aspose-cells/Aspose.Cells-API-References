---
title: "Walls.GetCubePointYPx"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Walls-Methode. Gibt die y‑Koordinate des Scheitelpunkts des Walls‑Würfels zurück, nachdem die Chart.Calculate‑Methode aufgerufen wurde. Die Anzahl der Scheitelpunkte des Walls‑Würfels beträgt acht."
type: docs
url: /de/net/aspose.cells.charts/walls/getcubepointypx/
---
## Walls.GetCubePointYPx method

Liest die y‑Koordinate des Scheitelpunkts des Wandwürfels nach Aufruf der Methode Chart.Calculate(). Die Anzahl der Scheitelpunkte des Wandwürfels beträgt acht.

```csharp
public float GetCubePointYPx(int index)
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class WallsMethodGetCubePointYPxDemo
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

            // Füge ein 3D‑Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Berechne das Diagramm, um sicherzustellen, dass Wall‑Eigenschaften gefüllt sind
            chart.Calculate();

            // Hole das Walls‑Objekt
            Walls walls = chart.Walls;

            try
            {
                // Hole die Anzahl der Würfelpunkte
                int pointCount = walls.GetCubePointCount();

                if (pointCount > 0)
                {
                    // Rufe GetCubePointYPx mit dem ersten Index (0) auf
                    float yPx = walls.GetCubePointYPx(0);
                    Console.WriteLine($"Y-coordinate of first cube point in pixels: {yPx}");
                }
                else
                {
                    Console.WriteLine("No cube points available in the walls.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCubePointYPx method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("WallsMethodGetCubePointYPxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


