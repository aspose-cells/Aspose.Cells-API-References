---
title: "Trendline.Period"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Trendline özelliği. Hareketli ortalama trend çizgisi için dönemi döndürür veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/trendline/period/
---
## Trendline.Period property

Hareketli ortalama trend çizgisi için periyodu döndürür veya ayarlar.

```csharp
public int Period { get; set; }
```

### Açıklamalar

Bu değer 2 ile 255 arasında olmalıdır. Ayrıca serideki grafik noktalarının sayısından daha az olmalıdır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyPeriodDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
            }

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Seri ekle
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Bir hareketli ortalama trend çizgisi ekleyin
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.MovingAverage);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Period = 3; // Set period for moving average
            trendline.Name = "3-Period Moving Average";

            // Çalışma kitabını kaydedin
            workbook.Save("TrendlinePeriodDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


