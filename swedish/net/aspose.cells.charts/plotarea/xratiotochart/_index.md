---
title: "PlotArea.XRatioToChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PlotArea‑egenskap. Hämtar eller anger x‑koordinaten för det övre vänstra hörnet av plotområdets avgränsningsruta som ett förhållande till diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/plotarea/xratiotochart/
---
## PlotArea.XRatioToChart property

Hämtar eller anger x-koordinaten för det övre vänstra hörnet av plotområdets avgränsningsruta som ett förhållande till diagramområdet.

```csharp
public override double XRatioToChart { get; set; }
```

### Anmärkningar

Plotarea-omslutningsrutan inkluderar plotområdet, stapelmärken (stapelmärkesetiketter) och en liten kant runt stapelmärkena. Om värdet inte skapats av MS Excel, vänligen anropa metoden Chart.Calculate() innan du anropar denna metod.

De **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** och **HeightRatioToChart** för **PlotArea** representerar plot‑områdets avgränsningsruta som inkluderar plotområdet, staplar (stapeltiketter) och en liten kant runt staplarna. Om du vill få den faktiska storleken på plotområdet bör du anropa egenskaperna **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** och **InnerHeightRatioToChart**.

För Excel 2007 eller senare är standardvärdet noll. Du bör hämta värdet efter att ha anropat Chart.Calculate().

XPixel = XRatioToChart * chart.ChartObject.Width. Obs: När XRatioToChart anges, kommer egenskapen IsInnerMode automatiskt att sättas till false.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyXRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Hämta plot‑området för diagrammet
            PlotArea plotArea = chart.PlotArea;

            // Visa det aktuella XRatioToChart‑värdet
            Console.WriteLine("Current XRatioToChart value: " + plotArea.XRatioToChart);

            // Ändra XRatioToChart‑värdet för att flytta plotområdet horisontellt
            plotArea.XRatioToChart = 0.2; // 20% from the left of the chart area

            // Visa det nya XRatioToChart‑värdet
            Console.WriteLine("New XRatioToChart value: " + plotArea.XRatioToChart);

            // Spara arbetsboken för att se effekten
            workbook.Save("PlotAreaXRatioToChartDemo.xlsx");
        }
    }
}
```

### Se även

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


