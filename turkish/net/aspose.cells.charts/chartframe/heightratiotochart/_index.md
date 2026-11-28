---
title: "ChartFrame.HeightRatioToChart"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartFrame özelliği. Çerçevenin yüksekliğini grafik alanının oranı biriminde alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/chartframe/heightratiotochart/
---
## ChartFrame.HeightRatioToChart property

Çerçevenin yüksekliğini, çizelge alanının oran biriminde alır veya ayarlar.

```csharp
public virtual double HeightRatioToChart { get; set; }
```

### Açıklamalar

Bu bir kesir değeridir, geçerli aralığı 0-1 arasındadır. Oran birimlerini piksel'e nasıl dönüştürülür? HeightPixel = HeightRatioToChart * Chart.ChartObject.Height;

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyHeightRatioToChartDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafik başlığına erişin (ChartFrame'den miras alır)
            chart.Title.Text = "Sample Chart";
            ChartFrame titleFrame = chart.Title;

            // Mevcut HeightRatioToChart değerini göster
            Console.WriteLine("Current HeightRatioToChart value: " + titleFrame.HeightRatioToChart);

            // Yeni bir yükseklik oranı ayarla (0.1 = grafik yüksekliğinin %10'u)
            titleFrame.HeightRatioToChart = 0.1;

            // Öncesi/sonrası karşılaştırarak etkiyi göster
            Console.WriteLine("Title height reduced to 10% of chart height");

            // Sonucu kaydet
            workbook.Save("PropertyHeightRatioToChartDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


