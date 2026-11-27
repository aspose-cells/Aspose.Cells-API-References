---
title: "PlotArea.InnerHeightRatioToChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PlotArea‑egenskap. Hämtar eller sätter höjden på plot‑området i enheter av förhållandet till diagramområdet."
type: docs
url: /sv/net/aspose.cells.charts/plotarea/innerheightratiotochart/
---
## PlotArea.InnerHeightRatioToChart property

Hämtar eller anger höjden på plotområdet i enheter av förhållandet till diagramområdet.

```csharp
public double InnerHeightRatioToChart { get; set; }
```

### Anmärkningar

Plotarea-omslutningsrutan inkluderar plotområdet, stapelmärken (stapelmärkesetiketter) och en liten kant runt stapelmärkena. Om värdet inte skapats av MS Excel, vänligen anropa metoden Chart.Calculate() innan du anropar denna metod.

De **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** och **HeightRatioToChart** för **PlotArea** representerar plot‑områdets avgränsningsruta som inkluderar plotområdet, staplar (stapeltiketter) och en liten kant runt staplarna. Om du vill få den faktiska storleken på plotområdet bör du anropa egenskaperna **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** och **InnerHeightRatioToChart**.

För Excel 2007 eller senare är standardvärdet noll. Du bör hämta värdet efter att ha anropat Chart.Calculate().

InnerHeight i pixel = InnerXRatioToChart * chart.ChartObject.Width. Obs: När InnerHeightRatioToChart sätts kommer egenskapen IsInnerMode automatiskt att sättas till True.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyInnerHeightRatioToChartDemo
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

            // Åtkomst till plot‑området
            PlotArea plotArea = chart.PlotArea;

            // Visa aktuellt värde för InnerHeightRatioToChart
            Console.WriteLine("Current InnerHeightRatioToChart value: " + plotArea.InnerHeightRatioToChart);

            // Ange ett nytt värde för InnerHeightRatioToChart (0.5 = 50 % av diagramområdets höjd)
            plotArea.InnerHeightRatioToChart = 0.5;

            // Visa effekten genom att spara arbetsboken
            workbook.Save("PlotAreaInnerHeightRatioToChartDemo.xlsx");

            // Visa nytt värde
            Console.WriteLine("New InnerHeightRatioToChart value: " + plotArea.InnerHeightRatioToChart);
        }
    }
}
```

### Se även

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


