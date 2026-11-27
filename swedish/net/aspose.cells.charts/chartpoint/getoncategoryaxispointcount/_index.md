---
title: "ChartPoint.GetOnCategoryAxisPointCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint‑metod. Hämtar antalet punkter på kategori‑axeln efter anrop av Chart.Calculate‑metoden. Gäller endast för area‑diagram"
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/getoncategoryaxispointcount/
---
## ChartPoint.GetOnCategoryAxisPointCount method

Hämtar antalet punkter på kategorisaxeln efter att ha anropat metoden Chart.Calculate(). Gäller endast för områdesdiagram.

```csharp
public int GetOnCategoryAxisPointCount()
```

### Anmärkningar

Area 2D-diagram returnerar 1, Area 3D-diagram returnerar 2.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetOnCategoryAxisPointCountDemo
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

            // Lägg till ett area‑diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet för att säkerställa att alla diagrampunkter beräknas
            chart.Calculate();

            try
            {
                // Hämta den första diagrampunkten från den första serien
                ChartPoint point = chart.NSeries[0].Points[0];
                
                // Anropa GetOnCategoryAxisPointCount‑metoden
                int pointCount = point.GetOnCategoryAxisPointCount();
                
                Console.WriteLine($"Number of points on category axis: {pointCount}");
                
                // Visa koordinaterna för varje punkt på kategori‑axeln
                for (int i = 0; i < pointCount; i++)
                {
                    float x = point.GetOnCategoryAxisPointXPx(i);
                    float y = point.GetOnCategoryAxisPointYPx(i);
                    Console.WriteLine($"Point {i}: X={x}, Y={y}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOnCategoryAxisPointCount method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("MethodGetOnCategoryAxisPointCountDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


