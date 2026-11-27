---
title: "Title.YRatioToChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Title-egenskapen. Hämtar eller anger y-koordinaten för det övre vänstra hörnet i enheter av bråkdel av diagramområdet. Y i pixlar  YRatioToChart  Chart.ChartObject.Width"
type: docs
url: /sv/net/aspose.cells.charts/title/yratiotochart/
---
## Title.YRatioToChart property

Hämtar eller anger y‑koordinaten för det övre vänstra hörnet i enheter av bråkdel av diagramområdet. Y i pixlar = YRatioToChart * Chart.ChartObject.Width;

```csharp
public override double YRatioToChart { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TitlePropertyYRatioToChartDemo
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

            // Hämta diagramtitel
            chart.Title.Text = "Sample Chart Title";
            Title chartTitle = chart.Title;

            // Visa aktuellt YRatioToChart-värde
            Console.WriteLine("Current YRatioToChart value: " + chartTitle.YRatioToChart);

            // Ändra YRatioToChart-egenskapen för att flytta titeln vertikalt
            chartTitle.YRatioToChart = 0.1; // 10% from the top of the chart area
            Console.WriteLine("New YRatioToChart value: " + chartTitle.YRatioToChart);

            // Spara arbetsboken
            workbook.Save("TitlePropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### Se även

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


