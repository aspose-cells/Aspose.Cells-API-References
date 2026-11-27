---
title: "PlotArea.HeightRatioToChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PlotArea‑egenskap. Hämtar eller anger höjden på plotområdets avgränsningsruta i enheter av förhållandet till diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/plotarea/heightratiotochart/
---
## PlotArea.HeightRatioToChart property

Hämtar eller anger höjden på plotområdets avgränsningsruta i enheter av förhållandet till diagramområdet.

```csharp
public override double HeightRatioToChart { get; set; }
```

### Anmärkningar

Plotarea-omslutningsrutan inkluderar plotområdet, stapelmärken (stapelmärkesetiketter) och en liten kant runt stapelmärkena. Om värdet inte skapats av MS Excel, vänligen anropa metoden Chart.Calculate() innan du anropar denna metod.

De **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** och **HeightRatioToChart** för **PlotArea** representerar plot‑områdets avgränsningsruta som inkluderar plotområdet, staplar (stapeltiketter) och en liten kant runt staplarna. Om du vill få den faktiska storleken på plotområdet bör du anropa egenskaperna **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** och **InnerHeightRatioToChart**.

För Excel 2007 eller senare är standardvärdet noll. Du bör hämta värdet efter att ha anropat Chart.Calculate().

HeightPixel = HeightRatioToChart * chart.ChartObject.Width. Obs: När HeightRatioToChart anges, kommer egenskapen IsInnerMode automatiskt att sättas till false.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyHeightRatioToChartDemo
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
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Hämta plot‑området för diagrammet
            PlotArea plotArea = chart.PlotArea;

            // Visa det aktuella höjdförhållandet
            Console.WriteLine("Current HeightRatioToChart value: " + plotArea.HeightRatioToChart);

            // Ställ in ett nytt höjdförhållande (0,7 betyder 70 % av diagramområdets höjd)
            plotArea.HeightRatioToChart = 0.7;

            // Visa det nya höjdförhållandet
            Console.WriteLine("New HeightRatioToChart value: " + plotArea.HeightRatioToChart);

            // Spara arbetsboken för att se effekten
            workbook.Save("PlotAreaHeightRatioToChartDemo.xlsx");
        }
    }
}
```

### Se även

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


