---
title: "AxisBins.Width"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AxisBins egenskap. Hämtar eller anger bredden på axelbehållaren"
type: docs
url: /sv/net/aspose.cells.charts/axisbins/width/
---
## AxisBins.Width property

Hämtar eller anger bredden på axis bin.

```csharp
public double Width { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisBinsPropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exempeldata
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["C1"].PutValue(20);
            worksheet.Cells["D1"].PutValue(15);
            worksheet.Cells["B2"].PutValue(35);
            worksheet.Cells["C2"].PutValue(32);
            worksheet.Cells["D2"].PutValue(31);

            // Skapa histogramdiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Histogram, 7, 1, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:D2", false);
            chart.NSeries.CategoryData = "B1:D1";

            // Ställ in behållarbredd
            chart.CategoryAxis.Bins.Width = 12;

            // Spara och demonstrera resultatet
            workbook.Save("AxisBinsPropertyWidthDemo_out.xlsx");

            Console.WriteLine("Example executed successfully with bin width set to 12.");
        }
    }
}
```

### Se även

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


