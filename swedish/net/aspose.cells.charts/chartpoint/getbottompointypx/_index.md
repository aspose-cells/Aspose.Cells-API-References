---
title: "ChartPoint.GetBottomPointYPx"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint-metod. Hämtar y-koordinaten för den nedre punkten på formen efter anrop av Chart.Calculate-metoden. Gäller 3D-diagram Column3D Bar3D Cone Cylinder Pyramid."
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/getbottompointypx/
---
## ChartPoint.GetBottomPointYPx method

Hämtar y‑koordinaten för den nedre punkten i formen efter att ha anropat metoden Chart.Calculate(). Gäller för 3D‑diagram: Column3D, Bar3D, Cone, Cylinder, Pyramid.

```csharp
public float GetBottomPointYPx(int index)
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetBottomPointYPxDemo
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
            
            // Lägg till serie
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Beräkna diagrammet för att säkerställa att alla punkter beräknas
            chart.Calculate();
            
            // Hämta den första punkten i den första serien
            ChartPoint point = chart.NSeries[0].Points[0];
            
            try
            {
                // Hämta antalet nedre punkter
                int bottomPointCount = point.GetBottomPointCount();
                
                if (bottomPointCount > 0)
                {
                    // Anropa GetBottomPointYPx med index 0
                    float yPx = point.GetBottomPointYPx(0);
                    
                    Console.WriteLine($"Bottom point Y position in pixels: {yPx}");
                    Console.WriteLine("Method executed successfully with parameter (Int32)");
                }
                else
                {
                    Console.WriteLine("No bottom points available for this chart point");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBottomPointYPx method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("MethodGetBottomPointYPxDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


