---
title: "Walls.GetCubePointXPx"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Walls-metod. Hämtar x-koordinaten för spetsen på väggkubens toppunkt efter att ha anropat metoden Chart.Calculate. Antalet spetspunkter på väggkuben är åtta."
type: docs
url: /sv/net/aspose.cells.charts/walls/getcubepointxpx/
---
## Walls.GetCubePointXPx method

Hämtar x-koordinaten för apex-punkten i väggkuben efter att ha anropat metoden Chart.Calculate(). Antalet apex-punkter i väggkuben är åtta

```csharp
public float GetCubePointXPx(int index)
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
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

            // Skapa ett 3D-diagram.
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Beräkna diagrammet för att säkerställa att Wall‑egenskaperna är tillgängliga
            chart.Calculate();

            // Hämta Walls‑objektet
            Walls walls = chart.Walls;

            try
            {
                // Hämta antalet kubpunkter.
                int pointCount = walls.GetCubePointCount();

                if (pointCount > 0)
                {
                    // Anropa GetCubePointXPx med index 0 (första punkten).
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

            // Spara arbetsboken
            workbook.Save("WallsMethodGetCubePointXPxDemo.xlsx");
        }
    }
}
```

### Se även

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


