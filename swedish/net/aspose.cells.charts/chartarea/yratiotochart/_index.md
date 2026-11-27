---
title: "ChartArea.YRatioToChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartArea-egenskap. Hämtar eller anger det vertikala offsetet från dess övre vänstra hörnrad i enheter av förhållandet till diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/chartarea/yratiotochart/
---
## ChartArea.YRatioToChart property

Hämtar eller hämtar det vertikala offsetet från dess övre vänstra hörnrad, i enheter av förhållandet till diagramområdet.

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

    public class ChartAreaPropertyYRatioToChartDemo
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
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Åtkomst till diagramområdet
            ChartArea chartArea = chart.ChartArea;

            // Visa det aktuella YRatioToChart‑värdet
            Console.WriteLine("Current YRatioToChart value: " + chartArea.YRatioToChart);

            // Ändra YRatioToChart‑egenskapen (0,0 till 1,0 representerar 0 % till 100 % av diagramområdet)
            chartArea.YRatioToChart = 0.2; // Move chart area down by 20% of chart height

            // Visa det nya YRatioToChart‑värdet
            Console.WriteLine("New YRatioToChart value: " + chartArea.YRatioToChart);

            // Spara arbetsboken för att se effekten
            workbook.Save("ChartAreaPropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


