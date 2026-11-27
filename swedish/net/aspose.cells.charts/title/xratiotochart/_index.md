---
title: "Title.XRatioToChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Title-egenskapen. Hämtar eller anger x-koordinaten för det övre vänstra hörnet i enheter av bråkdel av diagramområdet. X i pixlar  XRatioToChart  Chart.ChartObject.Width"
type: docs
url: /sv/net/aspose.cells.charts/title/xratiotochart/
---
## Title.XRatioToChart property

Hämtar eller anger x‑koordinaten för det övre vänstra hörnet i enheter av bråkdel av diagramområdet. X i pixlar = XRatioToChart * Chart.ChartObject.Width;

```csharp
public override double XRatioToChart { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TitlePropertyXRatioToChartDemo
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

            // Ange datakälla för diagrammet
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Hämta diagramtitel
            chart.Title.Text = "Sample Chart Title";
            Title title = chart.Title;

            // Visa aktuellt XRatioToChart‑värde
            Console.WriteLine("Current XRatioToChart value: " + title.XRatioToChart);

            // Ändra XRatioToChart‑värdet för att flytta titeln horisontellt
            title.XRatioToChart = 0.25; // 25% from the left of the chart area
            Console.WriteLine("New XRatioToChart value: " + title.XRatioToChart);

            // Spara arbetsboken
            workbook.Save("TitlePropertyXRatioToChartDemo.xlsx");
        }
    }
}
```

### Se även

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


