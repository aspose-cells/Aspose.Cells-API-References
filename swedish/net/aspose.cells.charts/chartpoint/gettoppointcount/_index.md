---
title: "ChartPoint.GetTopPointCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint‑metod. Hämtar antalet övre punkter efter att Chart.Calculate‑metoden har anropats"
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/gettoppointcount/
---
## ChartPoint.GetTopPointCount method

Hämtar antalet övre punkter efter att ha anropat metoden Chart.Calculate().

```csharp
public int GetTopPointCount()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetTopPointCountDemo
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

            // Lägg till ett stapeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet för att säkerställa att alla egenskaper är satta
            chart.Calculate();

            try
            {
                // Hämta den första punkten i den första serien.
                ChartPoint point = chart.NSeries[0].Points[0];
                
                // Anropa GetTopPointCount-metoden
                int topPointCount = point.GetTopPointCount();
                
                // Visa resultatet
                Console.WriteLine($"Number of top points: {topPointCount}");
                
                // Demonstrera hur man hämtar toppunktens koordinater
                if (topPointCount > 0)
                {
                    for (int i = 0; i < topPointCount; i++)
                    {
                        float x = point.GetTopPointXPx(i);
                        float y = point.GetTopPointYPx(i);
                        Console.WriteLine($"Top point {i + 1} coordinates: ({x}, {y})");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTopPointCount method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("MethodGetTopPointCountDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


