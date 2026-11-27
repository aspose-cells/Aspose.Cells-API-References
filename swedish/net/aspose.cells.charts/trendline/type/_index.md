---
title: "Trendline.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Trendline-egenskap. Returnerar trendlinjetypen"
type: docs
url: /sv/net/aspose.cells.charts/trendline/type/
---
## Trendline.Type property

Returnerar trendlinjetypen.

```csharp
public TrendlineType Type { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["A5"].PutValue(4);
            
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["B2"].PutValue(2);
            sheet.Cells["B3"].PutValue(4);
            sheet.Cells["B4"].PutValue(8);
            sheet.Cells["B5"].PutValue(16);

            // Lägg till ett diagram
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Lägg till serie
            chart.NSeries.Add("A2:A5", true);
            chart.NSeries[0].XValues = "B2:B5";

            // Lägg till exponentiell trendlinje
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Exponential);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Demonstrera användning av Type-egenskapen
            Console.WriteLine("Trendline type: " + trendline.Type);
            
            // Spara arbetsboken
            workbook.Save("TrendlinePropertyTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TrendlineType](../../trendlinetype/)
* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


