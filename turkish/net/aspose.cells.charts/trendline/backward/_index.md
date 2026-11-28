---
title: "Trendline.Backward"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Trendline özelliği. Trend çizgisinin geriye doğru uzandığı dağılım grafiğindeki dönem veya birim sayısını döndürür veya ayarlar. Dönem sayısı sıfırdan büyük veya eşit olmalıdır. Grafik tipi sütun ise dönem sayısı 0 ile 0.5 arasında olmalıdır."
type: docs
url: /tr/net/aspose.cells.charts/trendline/backward/
---
## Trendline.Backward property

Trend çizgisinin geriye doğru uzadığı dönem (veya dağılım grafiğindeki birimler) sayısını döndürür veya ayarlar. Dönem sayısı sıfırdan büyük veya eşit olmalıdır. Grafik türü sütun ise, dönem sayısı 0 ile 0,5 arasında olmalıdır.

```csharp
public double Backward { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyBackwardDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);

            // Grafik oluştur
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);

            // Trend çizgisi ekleyin ve indeksle alın
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(Aspose.Cells.Charts.TrendlineType.Linear);
            Aspose.Cells.Charts.Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "Linear Trend";
            trendline.DisplayEquation = true;
            
            // Trend çizgisini geriye doğru 0.5 birim uzatmak için backward özelliğini ayarlayın
            trendline.Backward = 0.5;
            
            workbook.Save("TrendlineBackwardDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


