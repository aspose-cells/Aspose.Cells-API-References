---
title: "Trendline.Forward"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Trendline-egenskap. Returnerar eller anger antalet perioder eller enheter i ett spridningsdiagram som trendlinjen sträcker sig framåt. Antalet perioder måste vara större än eller lika med noll."
type: docs
url: /sv/net/aspose.cells.charts/trendline/forward/
---
## Trendline.Forward property

Returnerar eller anger antalet perioder (eller enheter i ett spridningsdiagram) som trendlinjen sträcker sig framåt. Antalet perioder måste vara större än eller lika med noll.

```csharp
public double Forward { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyForwardDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Lägg till diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Lägg till trendlinje
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "Linear Trend";
            trendline.DisplayEquation = true;
            
            // Demonstrera Forward-egenskapen
            trendline.Forward = 2.5; // Extend trendline forward by 2.5 units
            
            workbook.Save("TrendlineForwardDemo.xlsx");
        }
    }
}
```

### Se även

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


