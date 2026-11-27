---
title: "Walls.GetCubePointCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Walls‑metoden. Hämtar antalet kubpunkter efter anrop av metoden Chart.Calculate."
type: docs
url: /sv/net/aspose.cells.charts/walls/getcubepointcount/
---
## Walls.GetCubePointCount method

Hämtar antalet kubpunkter efter anrop av metoden Chart.Calculate().

```csharp
public int GetCubePointCount()
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett 3D-diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet för att säkerställa att Wall‑egenskaperna är tillgängliga
            chart.Calculate();

            try
            {
                // Hämta Walls‑objektet
                Walls walls = chart.Walls;
                
                // Anropa metoden GetCubePointCount
                int pointCount = walls.GetCubePointCount();
                
                // Visa resultatet
                Console.WriteLine($"Number of cube points in chart walls: {pointCount}");
                
                // Spara arbetsboken
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

### Se även

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


