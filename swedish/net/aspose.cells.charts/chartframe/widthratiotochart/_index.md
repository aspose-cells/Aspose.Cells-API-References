---
title: "ChartFrame.WidthRatioToChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame‑egenskap. Hämtar eller anger bredden på ramen i enheter av förhållandet till diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/widthratiotochart/
---
## ChartFrame.WidthRatioToChart property

Hämtar eller anger bredden på ramen i förhållande till diagramområdet.

```csharp
public virtual double WidthRatioToChart { get; set; }
```

### Anmärkningar

Detta är ett bråkvärde, dess giltiga intervall är mellan 0‑1. Hur konverterar man förhållandeenheter till pixlar? WidthPixel = WidthRatioToChart * Chart.ChartObject.Width;

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyWidthRatioToChartDemo
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

            // Visa det aktuella breddförhållandet
            Console.WriteLine("Current WidthRatioToChart value: " + chartTitle.WidthRatioToChart);

            // Ange ett nytt breddförhållande (0,5 = 50 % av diagrambredden)
            chartTitle.WidthRatioToChart = 0.5;

            // Visa effekten genom att spara arbetsboken
            workbook.Save("ChartFrameWidthRatioDemo.xlsx");

            Console.WriteLine("WidthRatioToChart property demonstrated successfully.");
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


