---
title: "PlotArea.SetPositionAuto"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PlotArea-metod. Ställ in positionen för plotområdet till automatisk"
type: docs
url: /sv/net/aspose.cells.charts/plotarea/setpositionauto/
---
## PlotArea.SetPositionAuto method

Ställ in positionen för plotområdet till automatisk

```csharp
public override void SetPositionAuto()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaMethodSetPositionAutoDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Hämta plot‑området för diagrammet
                PlotArea plotArea = chart.PlotArea;
                
                // Ställ manuellt in några positionsvärden först för att demonstrera effekten
                plotArea.XRatioToChart = 0.1;
                plotArea.YRatioToChart = 0.1;
                plotArea.WidthRatioToChart = 0.8;
                plotArea.HeightRatioToChart = 0.8;
                
                // Anropa SetPositionAuto för att återställa till automatisk positionering
                plotArea.SetPositionAuto();
                
                Console.WriteLine("Plot area position has been set to automatic.");
                
                // Spara arbetsboken för att visa effekten
                workbook.Save("PlotAreaSetPositionAutoDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetPositionAuto method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


