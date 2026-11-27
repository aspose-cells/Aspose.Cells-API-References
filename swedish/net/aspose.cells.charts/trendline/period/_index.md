---
title: "Trendline.Period"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Trendline-egenskap. Returnerar eller anger perioden för den glidande medelvärdes-trendlinjen"
type: docs
url: /sv/net/aspose.cells.charts/trendline/period/
---
## Trendline.Period property

Returnerar eller anger perioden för glidande medelvärdes‑trendlinjen.

```csharp
public int Period { get; set; }
```

### Anmärkningar

Detta värde bör vara mellan 2 och 255. Och det måste vara mindre än antalet diagrampunkter i serien

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyPeriodDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
            }

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till serie
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Lägg till en glidande medelvärdes-trendlinje
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.MovingAverage);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Period = 3; // Set period for moving average
            trendline.Name = "3-Period Moving Average";

            // Spara arbetsboken
            workbook.Save("TrendlinePeriodDemo.xlsx");
        }
    }
}
```

### Se även

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


