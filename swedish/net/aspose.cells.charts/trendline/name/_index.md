---
title: "Trendline.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Trendline-egenskap. Returnerar namnet på trendlinjen"
type: docs
url: /sv/net/aspose.cells.charts/trendline/name/
---
## Trendline.Name property

Returnerar namnet på trendlinjen.

```csharp
public string Name { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyNameDemo
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
            
            // Lägg till serie i diagrammet
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Lägg till trendlinje och ange dess namn
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "My Custom Trendline";
            
            // Spara arbetsboken
            workbook.Save("TrendlinePropertyNameDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


