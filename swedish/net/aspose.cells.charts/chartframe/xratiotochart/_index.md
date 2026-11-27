---
title: "ChartFrame.XRatioToChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame-egenskap. Hämtar eller anger x-koordinaten för det övre vänstra hörnet i enheter av förhållandet till diagramområdet."
type: docs
url: /sv/net/aspose.cells.charts/chartframe/xratiotochart/
---
## ChartFrame.XRatioToChart property

Hämtar eller anger x‑koordinaten för det övre vänstra hörnet i förhållande till diagramområdet.

```csharp
public virtual double XRatioToChart { get; set; }
```

### Anmärkningar

Detta är ett bråkvärde, dess giltiga intervall är mellan 0‑1. Hur konverterar man enheter av förhållandet till pixlar? XPixel = XRatioToChart * Chart.ChartObject.Width;

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyXRatioToChartDemo
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

            // Åtkomst till diagramtiteln som är en ChartFrame
            ChartFrame chartTitle = chart.Title;

            // Visa aktuellt XRatioToChart‑värde
            Console.WriteLine("Current XRatioToChart value: " + chartTitle.XRatioToChart);

            // Ange nytt XRatioToChart‑värde (0,5 betyder 50 % av diagrambredden från vänster)
            chartTitle.XRatioToChart = 0.5;

            // Visa ny position
            Console.WriteLine("Title position after change - XRatioToChart: " + chartTitle.XRatioToChart);

            // Spara arbetsboken
            workbook.Save("ChartFrameXRatioToChartDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


