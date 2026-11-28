---
title: "AxisBins.IsAutomatic"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AxisBins özelliği. Eksen kutularının otomatik olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.charts/axisbins/isautomatic/
---
## AxisBins.IsAutomatic property

Eksen kutularının otomatik olup olmadığını gösterir.

```csharp
public bool IsAutomatic { get; set; }
```

### Açıklamalar

Eğer [`Width`](../width/) veya [`Count`](../count/) çağrılırsa, değer false olacaktır.

### Örnekler

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

            // IsAutomatic özelliğini gösterin
            bins.IsAutomatic = true;
            Console.WriteLine("Bins automatic calculation is enabled: " + bins.IsAutomatic);

            workbook.Save("AxisBinsIsAutomaticDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


