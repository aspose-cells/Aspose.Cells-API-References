---
title: "ChartPoint.GetTopPointXPx"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint metod. Hämtar x‑koordinaten för toppunkten på formen efter anrop av Chart.Calculate‑metoden. Gäller 3D‑diagram Column3D, Bar3D, Cone, Cylinder, Pyramid och Area3D"
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/gettoppointxpx/
---
## ChartPoint.GetTopPointXPx method

Hämtar x‑koordinaten för den övre punkten i formen efter att ha anropat metoden Chart.Calculate(). Gäller för 3D‑diagram: Column3D, Bar3D, Cone, Cylinder, Pyramid och Area3D.

```csharp
public float GetTopPointXPx(int index)
```

### Exempel

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

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet för att säkerställa att alla positions-egenskaper beräknas
            chart.Calculate();

            try
            {
                // Hämta den första diagrampunkten från den första serien
                ChartPoint point = chart.NSeries[0].Points[0];

                // Hämta antalet övre punkter
                int pointCount = point.GetTopPointCount();

                if (pointCount > 0)
                {
                    // Anropa GetTopPointXPx med index 0
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

            // Spara resultatet
            workbook.Save("ChartPointMethodGetTopPointXPxWithInt32Demo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


