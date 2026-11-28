---
title: "Axis.Bins"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Axis özelliği. Bir grafikHistogram/Pareto eksenindeki kutucukları temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/axis/bins/
---
## Axis.Bins property

Bir grafiğin (Histogram/Pareto) eksenindeki kutucukları temsil eder

```csharp
public AxisBins Bins { get; }
```

### Açıklamalar

Yalnızca Histogram veya Pareto grafiği için.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyBinsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Histogram grafiği oluştur
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Histogram, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A5", true);

            // Kutucukları yapılandır
            AxisBins bins = chart.ValueAxis.Bins;
            bins.IsAutomatic = false;
            bins.Width = 15;
            bins.Overflow = 55;
            bins.Underflow = 5;

            workbook.Save("AxisBinsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [AxisBins](../../axisbins/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


