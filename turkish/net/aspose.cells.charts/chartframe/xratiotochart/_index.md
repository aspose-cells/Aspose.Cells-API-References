---
title: "ChartFrame.XRatioToChart"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartFrame özelliği. Grafik alanının oran biriminde sol üst köşenin x koordinatını alır ve ayarlar."
type: docs
url: /tr/net/aspose.cells.charts/chartframe/xratiotochart/
---
## ChartFrame.XRatioToChart property

Üst sol köşenin x koordinatını, çizelge alanının oran biriminde alır veya ayarlar.

```csharp
public virtual double XRatioToChart { get; set; }
```

### Açıklamalar

Bu bir kesir değeridir, geçerli aralığı 0-1 arasındadır. Oran birimlerini piksele nasıl dönüştürülür? XPixel = XRatioToChart * Chart.ChartObject.Width;

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyXRatioToChartDemo
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

            // Mevcut XRatioToChart değerini göster
            Console.WriteLine("Current XRatioToChart value: " + chartTitle.XRatioToChart);

            // Yeni XRatioToChart değerini ayarla (0.5, soldan grafik genişliğinin %50'si anlamına gelir)
            chartTitle.XRatioToChart = 0.5;

            // Yeni konumu göster
            Console.WriteLine("Title position after change - XRatioToChart: " + chartTitle.XRatioToChart);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartFrameXRatioToChartDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


