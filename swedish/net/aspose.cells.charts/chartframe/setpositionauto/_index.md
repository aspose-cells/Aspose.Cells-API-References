---
title: "ChartFrame.SetPositionAuto"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame‑metod. Ställ in ramens position till automatisk"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/setpositionauto/
---
## ChartFrame.SetPositionAuto method

Ställ in ramens position till automatisk

```csharp
public virtual void SetPositionAuto()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFrameMethodSetPositionAutoDemo
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

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Hämta diagramrubrikens ram
            ChartFrame title = chart.Title;
            
            // Ställ in manuell position först för att demonstrera SetPositionAuto
            title.XRatioToChart = 0.2;
            title.YRatioToChart = 0.1;
            title.WidthRatioToChart = 0.6;
            title.HeightRatioToChart = 0.1;

            try
            {
                // Anropa SetPositionAuto‑metoden
                title.SetPositionAuto();
                
                Console.WriteLine("Chart title position set to automatic successfully");
                
                // Visa de nya automatiska positionsvärdena
                Console.WriteLine($"New X position ratio: {title.XRatioToChart}");
                Console.WriteLine($"New Y position ratio: {title.YRatioToChart}");
                Console.WriteLine($"New Width ratio: {title.WidthRatioToChart}");
                Console.WriteLine($"New Height ratio: {title.HeightRatioToChart}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetPositionAuto method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("ChartFrameSetPositionAutoDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


