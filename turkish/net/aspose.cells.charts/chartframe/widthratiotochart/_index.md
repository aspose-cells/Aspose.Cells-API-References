---
title: "ChartFrame.WidthRatioToChart"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartFrame özelliği. Çerçevenin genişliğini, grafik alanının oran biriminde alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/chartframe/widthratiotochart/
---
## ChartFrame.WidthRatioToChart property

Çerçevenin genişliğini, çizelge alanının oran biriminde alır veya ayarlar.

```csharp
public virtual double WidthRatioToChart { get; set; }
```

### Açıklamalar

Bu bir kesir değerdir, geçerli aralığı 0-1 arasındadır. Oran birimlerini piksellere nasıl dönüştürülür? WidthPixel = WidthRatioToChart * Chart.ChartObject.Width;

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyWidthRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // ChartFrame olan grafik başlığına erişin
            ChartFrame chartTitle = chart.Title;

            // Mevcut genişlik oranını göster
            Console.WriteLine("Current WidthRatioToChart value: " + chartTitle.WidthRatioToChart);

            // Yeni bir genişlik oranı ayarlayın (0.5 = grafiğin genişliğinin %50'si)
            chartTitle.WidthRatioToChart = 0.5;

            // Çalışma kitabını kaydederek etkiyi gösterin
            workbook.Save("ChartFrameWidthRatioDemo.xlsx");

            Console.WriteLine("WidthRatioToChart property demonstrated successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


