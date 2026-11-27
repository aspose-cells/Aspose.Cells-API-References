---
title: "TrendlineCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TrendlineCollection‑egenskap. Hämtar ett Trendline‑objekt efter dess index"
type: docs
url: /sv/net/aspose.cells.charts/trendlinecollection/item/
---
## TrendlineCollection indexer

Hämtar ett [`Trendline`](../../trendline/)‑objekt efter dess index.

```csharp
public Trendline this[int index] { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlineCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue(1);
            sheet.Cells["A2"].PutValue(2);
            sheet.Cells["A3"].PutValue(3);
            sheet.Cells["B1"].PutValue(4);
            sheet.Cells["B2"].PutValue(5);
            sheet.Cells["B3"].PutValue(6);

            // Lägg till ett diagram
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries[0].Values = "B1:B3";

            // Lägg till en trendlinje
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];

            // Demonstrera användning av Item-egenskapen
            Trendline firstTrendline = chart.NSeries[0].TrendLines[0];
            Console.WriteLine("Trendline Type: " + firstTrendline.Type);
        }
    }
}
```

### Se även

* class [Trendline](../../trendline/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


