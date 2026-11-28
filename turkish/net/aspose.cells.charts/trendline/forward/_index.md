---
title: "Trendline.Forward"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Trendline özelliği. Trend çizgisinin ileri doğru uzandığı dağılım grafiğindeki dönem veya birim sayısını döndürür veya ayarlar. Dönem sayısı sıfırdan büyük veya eşit olmalıdır."
type: docs
url: /tr/net/aspose.cells.charts/trendline/forward/
---
## Trendline.Forward property

Trend çizgisinin ileri doğru uzadığı dönem (veya dağılım grafiğindeki birimler) sayısını döndürür veya ayarlar. Dönem sayısı sıfırdan büyük veya eşit olmalıdır.

```csharp
public double Forward { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyForwardDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Trend çizgisi ekleyin
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "Linear Trend";
            trendline.DisplayEquation = true;
            
            // Forward özelliğini göster
            trendline.Forward = 2.5; // Extend trendline forward by 2.5 units
            
            workbook.Save("TrendlineForwardDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


