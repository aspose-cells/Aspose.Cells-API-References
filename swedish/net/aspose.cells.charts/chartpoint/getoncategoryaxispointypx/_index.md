---
title: "ChartPoint.GetOnCategoryAxisPointYPx"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint-metod. Hämtar y-koordinaten för punkten på kategoriaxeln efter att ha anropat metoden Chart.Calculate. Gäller endast för Area-diagram"
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/getoncategoryaxispointypx/
---
## ChartPoint.GetOnCategoryAxisPointYPx method

Hämtar y‑koordinaten för punkten på kategorisaxeln efter att ha anropat metoden Chart.Calculate(). Gäller endast för områdesdiagram.

```csharp
public float GetOnCategoryAxisPointYPx(int index)
```

### Anmärkningar

Area 2D-diagram: index är 0. Area 3D-diagram: index är 0 eller 1.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetOnCategoryAxisPointYPxWithInt32Demo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet för att säkerställa att alla positions-egenskaper beräknas
            chart.Calculate();

            // Hämta den första diagrampunkten från den första serien
            ChartPoint point = chart.NSeries[0].Points[0];

            try
            {
                // Anropa GetOnCategoryAxisPointYPx med index 0
                float yPx = point.GetOnCategoryAxisPointYPx(0);
                
                // Visa resultatet
                Console.WriteLine($"Y coordinate of point on category axis: {yPx} pixels");
                
                // Spara arbetsboken
                workbook.Save("ChartPointGetOnCategoryAxisPointYPxDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOnCategoryAxisPointYPx method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


