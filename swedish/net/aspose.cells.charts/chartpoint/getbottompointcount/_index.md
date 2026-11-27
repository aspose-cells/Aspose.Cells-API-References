---
title: "ChartPoint.GetBottomPointCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint‑metod. Hämtar antalet nedre punkter efter anrop av Chart.Calculate‑metoden"
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/getbottompointcount/
---
## ChartPoint.GetBottomPointCount method

Hämtar antalet nedre punkter efter att ha anropat metoden Chart.Calculate().

```csharp
public int GetBottomPointCount()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetBottomPointCountDemo
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
            
            // Beräkna diagrammet för att säkerställa att alla punkter beräknas
            chart.Calculate();
            
            try
            {
                // Hämta den första punkten i den första serien.
                ChartPoint point = chart.NSeries[0].Points[0];
                
                // Anropa GetBottomPointCount‑metoden
                int bottomPointCount = point.GetBottomPointCount();
                
                // Visa resultatet
                Console.WriteLine($"Number of bottom points: {bottomPointCount}");
                
                // Visa koordinaterna för de nedre punkterna
                for (int i = 0; i < bottomPointCount; i++)
                {
                    float x = point.GetBottomPointXPx(i);
                    float y = point.GetBottomPointYPx(i);
                    Console.WriteLine($"Bottom point {i}: X={x}, Y={y}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBottomPointCount method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("MethodGetBottomPointCountDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


