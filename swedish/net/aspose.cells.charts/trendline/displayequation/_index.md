---
title: "Trendline.DisplayEquation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Trendline-egenskap. Anger om ekvationen för trendlinjen visas på diagrammet i samma datamärkning som Rkvadrat-värdet. Att sätta denna egenskap till True aktiverar automatiskt datamärkningar"
type: docs
url: /sv/net/aspose.cells.charts/trendline/displayequation/
---
## Trendline.DisplayEquation property

Representerar om ekvationen för trendlinjen visas i diagrammet (i samma datamärkning som R‑kvadrerat‑värdet). Att sätta denna egenskap till True aktiverar automatiskt datamärkningar.

```csharp
public bool DisplayEquation { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyDisplayEquationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);

            // Skapa diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till serie och trendlinje
            chart.NSeries.Add("A1:B4", true);
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Konfigurera trendlinjeegenskaper
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = false;
            trendline.Color = Color.Blue;

            workbook.Save("TrendlineDisplayEquationDemo.xlsx");
        }
    }
}
```

### Se även

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


