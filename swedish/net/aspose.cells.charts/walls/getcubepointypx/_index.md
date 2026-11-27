---
title: "Walls.GetCubePointYPx"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Walls-metoden. Hämtar y‑koordinaten för apex‑punkten i väggarnas kub efter anrop av metoden Chart.Calculate. Antalet apex‑punkter i väggarnas kub är åtta"
type: docs
url: /sv/net/aspose.cells.charts/walls/getcubepointypx/
---
## Walls.GetCubePointYPx method

Hämtar y-koordinaten för apex-punkten i väggkuben efter anrop av metoden Chart.Calculate(). Antalet apex-punkter i väggkuben är åtta.

```csharp
public float GetCubePointYPx(int index)
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett 3D-diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet för att säkerställa att Wall‑egenskaperna är fyllda
            chart.Calculate();

            // Hämta Walls‑objektet
            Walls walls = chart.Walls;

            try
            {
                // Hämta antalet kubpunkter
                int pointCount = walls.GetCubePointCount();

                if (pointCount > 0)
                {
                    // Anropa GetCubePointYPx med det första indexet (0)
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

            // Spara arbetsboken
            workbook.Save("WallsMethodGetCubePointYPxDemo.xlsx");
        }
    }
}
```

### Se även

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


