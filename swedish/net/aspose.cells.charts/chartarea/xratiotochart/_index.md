---
title: "ChartArea.XRatioToChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartArea‑egenskap. Hämtar eller anger det horisontella offsetet från den övre vänstra kolumnen som ett förhållande till diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/chartarea/xratiotochart/
---
## ChartArea.XRatioToChart property

Hämtar eller anger det horisontella offsetet från den övre‑vänstra hörnkolumnen, som ett förhållande till diagramområdet.

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

    public class ChartAreaPropertyXRatioToChartDemo
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

            // Hämta diagramområdet
            ChartArea chartArea = chart.ChartArea;

            // Visa det aktuella XRatioToChart‑värdet
            Console.WriteLine("Current XRatioToChart value: " + chartArea.XRatioToChart);

            // Ändra XRatioToChart‑värdet för att flytta diagramområdet horisontellt
            chartArea.XRatioToChart = 0.2; // 20% from the left of the chart container

            // Visa det nya XRatioToChart‑värdet
            Console.WriteLine("New XRatioToChart value: " + chartArea.XRatioToChart);

            // Spara arbetsboken
            workbook.Save("ChartAreaXRatioToChartDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


