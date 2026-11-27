---
title: "Trendline.Intercept"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Trendline-egenskap. Returnerar eller anger den punkt där trendlinjen korsar värdeaxeln"
type: docs
url: /sv/net/aspose.cells.charts/trendline/intercept/
---
## Trendline.Intercept property

Returnerar eller anger punkten där trendlinjen korsar värdeaxeln.

```csharp
public double Intercept { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyInterceptDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(6);

            // Lägg till diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Lägg till trendlinje och ange intercept
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Intercept = 1.0; // Setting the Y-intercept value
            trendline.DisplayEquation = true;

            workbook.Save("TrendlineInterceptDemo.xlsx");
        }
    }
}
```

### Se även

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


