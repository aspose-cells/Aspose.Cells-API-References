---
title: "PlotArea.YRatioToChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PlotArea-egenskap. Hämtar eller anger y‑koordinaten för den övre hörnet av plotarea‑ramen som ett förhållande till diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/plotarea/yratiotochart/
---
## PlotArea.YRatioToChart property

Hämtar eller anger y-koordinaten för det övre hörnet av plot-områdets avgränsningsruta som ett förhållande till diagramområdet.

```csharp
public override double YRatioToChart { get; set; }
```

### Anmärkningar

Plotarea-omslutningsrutan inkluderar plotområdet, stapelmärken (stapelmärkesetiketter) och en liten kant runt stapelmärkena. Om värdet inte skapats av MS Excel, vänligen anropa metoden Chart.Calculate() innan du anropar denna metod.

De **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** och **HeightRatioToChart** för **PlotArea** representerar plot‑områdets avgränsningsruta som inkluderar plotområdet, staplar (stapeltiketter) och en liten kant runt staplarna. Om du vill få den faktiska storleken på plotområdet bör du anropa egenskaperna **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** och **InnerHeightRatioToChart**.

För Excel 2007 eller senare är standardvärdet noll. Du bör hämta värdet efter att ha anropat Chart.Calculate().

YPixel = YRatioToChart * chart.ChartObject.Width. Obs: När YRatioToChart anges, kommer egenskapen IsInnerMode automatiskt att sättas till false.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyYRatioToChartDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Hämta plot‑området för diagrammet
            PlotArea plotArea = chart.PlotArea;

            // Visa det aktuella YRatioToChart‑värdet
            Console.WriteLine("Current YRatioToChart value: " + plotArea.YRatioToChart);

            // Ange ett nytt YRatioToChart‑värde (0,1 betyder 10 % från toppen av diagramområdet)
            plotArea.YRatioToChart = 0.1;

            // Visa det nya YRatioToChart‑värdet
            Console.WriteLine("New YRatioToChart value: " + plotArea.YRatioToChart);

            // Spara arbetsboken för att se effekten
            workbook.Save("PlotAreaYRatioToChartDemo.xlsx");
        }
    }
}
```

### Se även

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


