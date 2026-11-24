---
title: "Walls.GetCubePointCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Walls‑Methode. Gibt die Anzahl der Würfelpunkte zurück, nachdem die Chart.Calculate‑Methode aufgerufen wurde."
type: docs
url: /de/net/aspose.cells.charts/walls/getcubepointcount/
---
## Walls.GetCubePointCount method

Liest die Anzahl der Würfelpunkte nach Aufruf der Methode Chart.Calculate().

```csharp
public int GetCubePointCount()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class WallsMethodGetCubePointCountDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Füge ein 3D‑Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Berechne das Diagramm, um sicherzustellen, dass Wall‑Eigenschaften verfügbar sind
            chart.Calculate();

            try
            {
                // Hole das Walls‑Objekt
                Walls walls = chart.Walls;
                
                // Rufe die GetCubePointCount‑Methode auf
                int pointCount = walls.GetCubePointCount();
                
                // Ergebnis anzeigen
                Console.WriteLine($"Number of cube points in chart walls: {pointCount}");
                
                // Speichere die Arbeitsmappe
                workbook.Save("WallsMethodGetCubePointCountDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCubePointCount method: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


