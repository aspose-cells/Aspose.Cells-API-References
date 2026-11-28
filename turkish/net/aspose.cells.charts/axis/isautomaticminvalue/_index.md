---
title: "Axis.IsAutomaticMinValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Axis özelliği. Minimum değerin otomatik olarak atanıp atanmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.charts/axis/isautomaticminvalue/
---
## Axis.IsAutomaticMinValue property

Minimum değerin otomatik olarak atanıp atanmayacağını belirtir.

```csharp
public bool IsAutomaticMinValue { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsAutomaticMinValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Değer eksenini yapılandır
            Axis valueAxis = chart.ValueAxis;
            valueAxis.IsAutomaticMinValue = false;
            valueAxis.MinValue = 0;
            valueAxis.IsAutomaticMaxValue = true; // Keep max value automatic for contrast
            
            // Sonucu kaydet
            workbook.Save("AxisPropertyIsAutomaticMinValueDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


