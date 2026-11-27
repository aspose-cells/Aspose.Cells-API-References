---
title: "Trendline.DisplayRSquared"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Trendline-egenskap. Anger om Rsquared‑värdet för trendlinjen visas i diagrammet i samma datamärkning som ekvationen. Att sätta denna egenskap till True aktiverar automatiskt datamärkningar."
type: docs
url: /sv/net/aspose.cells.charts/trendline/displayrsquared/
---
## Trendline.DisplayRSquared property

Representerar om R‑kvadrerat‑värdet för trendlinjen visas i diagrammet (i samma datamärkning som ekvationen). Att sätta denna egenskap till True aktiverar automatiskt datamärkningar.

```csharp
public bool DisplayRSquared { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyDisplayRSquaredDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].PutValue(4);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(6);
            worksheet.Cells["B4"].PutValue(8);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);

            // Lägg till en trendlinje och hämta den efter index
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "Linear Trend";
            
            // Demonstrera DisplayRSquared-egenskapen
            trendline.DisplayRSquared = true;
            trendline.DisplayEquation = true;

            // Spara arbetsboken
            workbook.Save("TrendlineDisplayRSquaredDemo.xlsx");
        }
    }
}
```

### Se även

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


