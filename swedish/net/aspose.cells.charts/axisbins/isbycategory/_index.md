---
title: "AxisBins.IsByCategory"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AxisBins egenskap. Anger om gruppering av data efter kategori är aktiverad"
type: docs
url: /sv/net/aspose.cells.charts/axisbins/isbycategory/
---
## AxisBins.IsByCategory property

Anger om gruppering av data efter kategori är aktiverad.

```csharp
public bool IsByCategory { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisBinsPropertyIsByCategoryDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["C1"].PutValue(20);
            worksheet.Cells["D1"].PutValue(15);
            worksheet.Cells["B2"].PutValue(35);
            worksheet.Cells["C2"].PutValue(32);
            worksheet.Cells["D2"].PutValue(31);
            worksheet.Cells["B3"].PutValue(185);
            worksheet.Cells["C3"].PutValue(202);
            worksheet.Cells["D3"].PutValue(224);

            // Lägg till histogramdiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Histogram, 7, 1, 25, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:D2", false);
            chart.NSeries.Add("B3:D3", false);
            chart.NSeries.CategoryData = "B1:D1";

            // Konfigurera axelbehållare
            Aspose.Cells.Charts.AxisBins bins = chart.CategoryAxis.Bins;
            bins.IsByCategory = false; // Explicitly set to false (default)
            bins.Width = 12;
            bins.Count = 3;
            bins.Overflow = 10;
            bins.Underflow = 0.5;

            // Spara och skriv ut resultatet
            workbook.Save("AxisBinsPropertyIsByCategoryDemo_output.xlsx");

            Console.WriteLine("IsByCategory: " + bins.IsByCategory);
            Console.WriteLine("Bin Width: " + bins.Width);
            Console.WriteLine("Bin Count: " + bins.Count);
            Console.WriteLine("Overflow: " + bins.Overflow);
            Console.WriteLine("Underflow: " + bins.Underflow);
        }
    }
}
```

### Se även

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


