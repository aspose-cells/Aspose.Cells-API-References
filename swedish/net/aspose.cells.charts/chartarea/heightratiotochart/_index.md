---
title: "ChartArea.HeightRatioToChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartArea-egenskap. Hämtar eller anger det vertikala offsetet från dess nedre högra hörnrad i enheter av förhållandet till diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/chartarea/heightratiotochart/
---
## ChartArea.HeightRatioToChart property

Hämtar eller anger det vertikala offsetet från dess nedre högra hörnrad, i enheter av förhållandet till diagramområdet.

```csharp
public override double HeightRatioToChart { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartAreaPropertyHeightRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Åtkomst till diagramområdet
            ChartArea chartArea = chart.ChartArea;

            // Visa det aktuella HeightRatioToChart‑värdet
            Console.WriteLine("Current HeightRatioToChart value: " + chartArea.HeightRatioToChart);

            // Ange ett nytt värde för HeightRatioToChart (0,5 = 50 % av diagramhöjden)
            chartArea.HeightRatioToChart = 0.5;
            Console.WriteLine("New HeightRatioToChart value: " + chartArea.HeightRatioToChart);

            // Ange ett nytt värde för WidthRatioToChart för att demonstrera kombinerad effekt
            chartArea.WidthRatioToChart = 0.8;

            // Spara workbook för att se ändringarna
            workbook.Save("ChartAreaPropertyHeightRatioToChartDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


