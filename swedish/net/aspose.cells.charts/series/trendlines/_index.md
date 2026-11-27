---
title: "Series.TrendLines"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Returnerar alla trendlinjer för denna serie"
type: docs
url: /sv/net/aspose.cells.charts/series/trendlines/
---
## Series.TrendLines property

Returnerar alla trendlinjer för denna serie.

```csharp
public TrendlineCollection TrendLines { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyTrendLinesDemo
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
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Lägg till en exponentiell trendlinje till den första serien och hämta den med index
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Exponential);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = true;

            // Spara arbetsboken
            workbook.Save("TrendLinesDemo.xlsx");
        }
    }
}
```

### Se även

* class [TrendlineCollection](../../trendlinecollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


