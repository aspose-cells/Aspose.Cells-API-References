---
title: "AxisBins.IsAutomatic"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AxisBins. تشير إلى ما إذا كانت صناديق المحور تلقائية"
type: docs
url: /ar/net/aspose.cells.charts/axisbins/isautomatic/
---
## AxisBins.IsAutomatic property

يشير إلى ما إذا كانت حاويات المحور تلقائية.

```csharp
public bool IsAutomatic { get; set; }
```

### ملاحظات

إذا تم استدعاء [`Width`](../width/) أو [`Count`](../count/)، ستكون القيمة false.

### أمثلة

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

            // إظهار خاصية IsAutomatic
            bins.IsAutomatic = true;
            Console.WriteLine("Bins automatic calculation is enabled: " + bins.IsAutomatic);

            workbook.Save("AxisBinsIsAutomaticDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


