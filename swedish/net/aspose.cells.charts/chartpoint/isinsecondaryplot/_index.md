---
title: "ChartPoint.IsInSecondaryPlot"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint-egenskap. Hämtar eller anger ett värde som visar om denna datapunkt finns i den andra pajen eller stapeln i ett paj‑i‑paj‑ eller stapel‑i‑paj‑diagram"
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/isinsecondaryplot/
---
## ChartPoint.IsInSecondaryPlot property

Hämtar eller anger ett värde som indikerar om denna datapunkt finns i den andra pajen eller stapeln i ett paj‑i‑paj‑eller‑stapel‑i‑paj‑diagram.

```csharp
public bool IsInSecondaryPlot { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyIsInSecondaryPlotDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Skapa ett pajdiagram som stöder sekundära diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Konfigurera sekundärt diagram
            chart.NSeries[0].Points[2].IsInSecondaryPlot = true;
            chart.NSeries[0].Points[3].IsInSecondaryPlot = true;

            // Spara utdata
            workbook.Save("PieChartWithSecondaryPlot.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


