---
title: "Trendline.Backward"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Trendline-egenskap. Returnerar eller anger antalet perioder eller enheter i ett spridningsdiagram som trendlinjen sträcker sig bakåt. Antalet perioder måste vara större än eller lika med noll. Om diagramtypen är kolumn måste antalet perioder vara mellan 0 och 0,5."
type: docs
url: /sv/net/aspose.cells.charts/trendline/backward/
---
## Trendline.Backward property

Returnerar eller anger antalet perioder (eller enheter i ett spridningsdiagram) som trendlinjen sträcker sig bakåt. Antalet perioder måste vara större än eller lika med noll. Om diagramtypen är kolumn, måste antalet perioder vara mellan 0 och 0,5

```csharp
public double Backward { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyBackwardDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);

            // Lägg till trendlinje och hämta den efter index
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(Aspose.Cells.Charts.TrendlineType.Linear);
            Aspose.Cells.Charts.Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "Linear Trend";
            trendline.DisplayEquation = true;
            
            // Ange backward-egenskapen för att förlänga trendlinjen bakåt med 0,5 enheter
            trendline.Backward = 0.5;
            
            workbook.Save("TrendlineBackwardDemo.xlsx");
        }
    }
}
```

### Se även

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


