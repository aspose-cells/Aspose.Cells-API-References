---
title: "ChartPoint.IsInSecondaryPlot"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. Bu veri noktasının pasta içinde ikinci pasta ya da çubukta olup olmadığını gösteren bir değeri alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/isinsecondaryplot/
---
## ChartPoint.IsInSecondaryPlot property

Bu veri noktasının pie of pie ya da bar of pie grafiğinde ikinci dilim ya da çubukta olup olmadığını gösteren bir değeri alır veya ayarlar.

```csharp
public bool IsInSecondaryPlot { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyIsInSecondaryPlotDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // İkincil çizimleri destekleyen bir pasta grafiği oluştur
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // İkincil çizimi yapılandır
            chart.NSeries[0].Points[2].IsInSecondaryPlot = true;
            chart.NSeries[0].Points[3].IsInSecondaryPlot = true;

            // Çıktıyı kaydet
            workbook.Save("PieChartWithSecondaryPlot.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


