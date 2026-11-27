---
title: "ChartFrame.YRatioToChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame-egenskap. Hämtar eller anger y-koordinaten för det övre vänstra hörnet i enheter av förhållandet för diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/yratiotochart/
---
## ChartFrame.YRatioToChart property

Hämtar eller anger y‑koordinaten för det övre vänstra hörnet i förhållande till diagramområdet.

```csharp
public virtual double YRatioToChart { get; set; }
```

### Anmärkningar

Detta är ett bråkvärde, dess giltiga intervall är mellan 0‑1. Hur konverterar man enheter av förhållandet till pixlar? YPixel = YRatioToChart * Chart.ChartObject.Height;

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyYRatioToChartDemo
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
            
            // Åtkomst till diagramtitel som ärver från ChartFrame
            chart.Title.Text = "Sample Chart";
            
            // Visa aktuellt YRatioToChart-värde
            Console.WriteLine("Current Title YRatioToChart value: " + chart.Title.YRatioToChart);
            
            // Ändra Y‑positionen för titeln i förhållande till diagramområdet
            chart.Title.YRatioToChart = 0.1; // 10% from top of chart area
            
            // Visa det nya YRatioToChart‑värdet
            Console.WriteLine("New Title YRatioToChart value: " + chart.Title.YRatioToChart);
            
            // Åtkomst till legenden som också ärver från ChartFrame
            chart.Legend.Position = LegendPositionType.Top;
            
            // Visa aktuellt YRatioToChart‑värde för legenden
            Console.WriteLine("Current Legend YRatioToChart value: " + chart.Legend.YRatioToChart);
            
            // Ändra Y‑positionen för legenden i förhållande till diagramområdet
            chart.Legend.YRatioToChart = 0.15; // 15% from top of chart area
            
            // Visa det nya YRatioToChart‑värdet för legenden
            Console.WriteLine("New Legend YRatioToChart value: " + chart.Legend.YRatioToChart);
            
            // Spara arbetsboken
            workbook.Save("ChartFramePropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


