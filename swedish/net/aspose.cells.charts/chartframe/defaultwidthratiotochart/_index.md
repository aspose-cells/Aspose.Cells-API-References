---
title: "ChartFrame.DefaultWidthRatioToChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame property. Representerar bredden för standardpositionen i enheter av en bråkdel av diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/defaultwidthratiotochart/
---
## ChartFrame.DefaultWidthRatioToChart property

Representerar bredden för standardpositionen i enheter av en bråkdel av diagramområdet.

```csharp
public double DefaultWidthRatioToChart { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultWidthRatioToChartDemo
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

            // Kom åt diagrammets titel som är ett ChartFrame
            ChartFrame chartTitle = chart.Title;

            // Visa det aktuella värdet för DefaultWidthRatioToChart
            Console.WriteLine("Current DefaultWidthRatioToChart value: " + chartTitle.DefaultWidthRatioToChart);

            // Obs: DefaultWidthRatioToChart är skrivskyddad, så vi kan inte ändra den
            // Istället kommer vi att demonstrera dess relation till det faktiska breddförhållandet
            Console.WriteLine("Current WidthRatioToChart: " + chartTitle.WidthRatioToChart);

            // Ändra breddförhållandet för att demonstrera dess effekt
            chartTitle.WidthRatioToChart = 0.5;
            Console.WriteLine("After setting WidthRatioToChart to 0.5, DefaultWidthRatioToChart remains: " + chartTitle.DefaultWidthRatioToChart);

            // Spara arbetsboken
            workbook.Save("ChartFramePropertyDefaultWidthRatioToChartDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


