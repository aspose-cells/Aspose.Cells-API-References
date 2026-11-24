---
title: "Walls.GetCubePointXPx"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Walls-Methode. Gibt die x‑Koordinate des Scheitelpunkts des Wandwürfels zurück, nachdem die Methode Chart.Calculate aufgerufen wurde. Die Anzahl der Scheitelpunkte des Wandwürfels beträgt acht."
type: docs
url: /de/net/aspose.cells.charts/walls/getcubepointxpx/
---
## Walls.GetCubePointXPx method

Liest die x‑Koordinate des Scheitelpunkts des Wandwürfels nach Aufruf der Methode Chart.Calculate(). Die Anzahl der Scheitelpunkte des Wandwürfels beträgt acht.

```csharp
public float GetCubePointXPx(int index)
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class WallsMethodGetCubePointXPxWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);
            worksheet.Cells["B5"].PutValue(4000);

            // Erstellen Sie ein 3D-Diagramm
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Berechne das Diagramm, um sicherzustellen, dass Wall‑Eigenschaften verfügbar sind
            chart.Calculate();

            // Hole das Walls‑Objekt
            Walls walls = chart.Walls;

            try
            {
                // Ermitteln Sie die Anzahl der Würfelpunkte
                int pointCount = walls.GetCubePointCount();

                if (pointCount > 0)
                {
                    // Rufen Sie GetCubePointXPx mit dem Index 0 (erster Punkt) auf
                    float xCoordinate = walls.GetCubePointXPx(0);
                    
                    Console.WriteLine($"X coordinate of first cube point in pixels: {xCoordinate}");
                    Console.WriteLine("Method executed successfully with parameter (Int32)");
                }
                else
                {
                    Console.WriteLine("No cube points available in the walls");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCubePointXPx method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("WallsMethodGetCubePointXPxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


