---
title: "ChartFrame.DefaultHeightRatioToChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame-egenskap. Representerar höjden för standardpositionen i enheter av andelen av diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/defaultheightratiotochart/
---
## ChartFrame.DefaultHeightRatioToChart property

Representerar höjden för standardpositionen i enheter av en bråkdel av diagramområdet.

```csharp
public double DefaultHeightRatioToChart { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultHeightRatioToChartDemo
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

            // Åtkomst till diagramtiteln (som är en ChartFrame)
            ChartFrame chartTitle = chart.Title;

            // Visa det aktuella DefaultHeightRatioToChart-värdet
            Console.WriteLine("Current DefaultHeightRatioToChart value: " + chartTitle.DefaultHeightRatioToChart);

            // Demonstrera hur denna egenskap påverkar diagrammet genom att jämföra med HeightRatioToChart
            Console.WriteLine("Current HeightRatioToChart value: " + chartTitle.HeightRatioToChart);

            // Ändra höjdförhållandet för att se effekten
            chartTitle.HeightRatioToChart = 0.1;
            Console.WriteLine("After setting HeightRatioToChart to 0.1: " + chartTitle.HeightRatioToChart);

            // Spara arbetsboken
            workbook.Save("ChartFramePropertyDefaultHeightRatioToChartDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


