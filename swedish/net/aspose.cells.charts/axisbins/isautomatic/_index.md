---
title: "AxisBins.IsAutomatic"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AxisBins egenskap. Anger om axelbehållarna är automatiska"
type: docs
url: /sv/net/aspose.cells.charts/axisbins/isautomatic/
---
## AxisBins.IsAutomatic property

Anger om axis bins är automatiska.

```csharp
public bool IsAutomatic { get; set; }
```

### Anmärkningar

Om [`Width`](../width/) eller [`Count`](../count/) anropas, blir värdet falskt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisBinsPropertyIsAutomaticDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Histogram, 5, 0, 25, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A5", true);

            Aspose.Cells.Charts.Axis valueAxis = chart.ValueAxis;
            Aspose.Cells.Charts.AxisBins bins = valueAxis.Bins;

            // Demonstrera IsAutomatic-egenskapen
            bins.IsAutomatic = true;
            Console.WriteLine("Bins automatic calculation is enabled: " + bins.IsAutomatic);

            workbook.Save("AxisBinsIsAutomaticDemo.xlsx");
        }
    }
}
```

### Se även

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


