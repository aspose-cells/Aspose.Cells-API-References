---
title: "ChartPoint.GetOnCategoryAxisPointXPx"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint-metod. Hämtar x-koordinaten för punkten på kategoriaxeln efter anrop av Chart.Calculate-metoden. Gäller endast för Area-diagram."
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/getoncategoryaxispointxpx/
---
## ChartPoint.GetOnCategoryAxisPointXPx method

Hämtar x‑koordinaten för punkten på kategorisaxeln efter att ha anropat metoden Chart.Calculate(). Gäller endast för områdesdiagram.

```csharp
public float GetOnCategoryAxisPointXPx(int index)
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

    public class ChartPointMethodGetOnCategoryAxisPointXPxWithInt32Demo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet
            chart.Calculate();

            try
            {
                // Hämta den första diagrampunkten
                ChartPoint point = chart.NSeries[0].Points[0];

                // Anropa GetOnCategoryAxisPointXPx med index 0
                float xPosition = point.GetOnCategoryAxisPointXPx(0);

                // Visa resultatet
                Console.WriteLine($"X position of first category axis point: {xPosition} pixels");

                // Spara arbetsboken
                workbook.Save("ChartPointGetOnCategoryAxisPointXPxDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOnCategoryAxisPointXPx method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


