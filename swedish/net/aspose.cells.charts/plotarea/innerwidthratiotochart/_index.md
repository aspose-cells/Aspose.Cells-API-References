---
title: "PlotArea.InnerWidthRatioToChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PlotArea‑egenskap. Hämtar eller anger bredden på plot‑området i enheter av förhållandet till diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/plotarea/innerwidthratiotochart/
---
## PlotArea.InnerWidthRatioToChart property

Hämtar eller anger bredden på plotområdet i enheter av förhållandet till diagramområdet.

```csharp
public double InnerWidthRatioToChart { get; set; }
```

### Anmärkningar

Plotarea-omslutningsrutan inkluderar plotområdet, stapelmärken (stapelmärkesetiketter) och en liten kant runt stapelmärkena. Om värdet inte skapats av MS Excel, vänligen anropa metoden Chart.Calculate() innan du anropar denna metod.

De **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** och **HeightRatioToChart** för **PlotArea** representerar plot‑områdets avgränsningsruta som inkluderar plotområdet, staplar (stapeltiketter) och en liten kant runt staplarna. Om du vill få den faktiska storleken på plotområdet bör du anropa egenskaperna **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** och **InnerHeightRatioToChart**.

För Excel 2007 eller senare är standardvärdet noll. Du bör hämta värdet efter att ha anropat Chart.Calculate().

InnerWidth i pixel = InnerXRatioToChart * chart.ChartObject.Width. Obs: När InnerWidthRatioToChart har angetts kommer egenskapen IsInnerMode automatiskt att sättas till True.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyInnerWidthRatioToChartDemo
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
            
            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Åtkomst till plot‑området
            PlotArea plotArea = chart.PlotArea;
            
            // Visa aktuellt InnerWidthRatioToChart‑värde
            Console.WriteLine("Current InnerWidthRatioToChart value: " + plotArea.InnerWidthRatioToChart);
            
            // Ange nytt värde för InnerWidthRatioToChart (0,5 betyder 50 % av diagrambredden)
            plotArea.InnerWidthRatioToChart = 0.5;
            
            // Visa effekten av ändringen
            Console.WriteLine("Plot area width changed to 50% of chart width");
            
            // Spara resultatet
            workbook.Save("PlotAreaPropertyInnerWidthRatioToChartDemo.xlsx");
        }
    }
}
```

### Se även

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


