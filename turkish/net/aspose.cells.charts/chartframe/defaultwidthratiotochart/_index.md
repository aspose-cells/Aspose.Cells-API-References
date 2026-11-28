---
title: "ChartFrame.DefaultWidthRatioToChart"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartFrame özelliği. Varsayılan konumun genişliğini, grafik alanının kesir birimi cinsinden temsil eder."
type: docs
url: /tr/net/aspose.cells.charts/chartframe/defaultwidthratiotochart/
---
## ChartFrame.DefaultWidthRatioToChart property

Varsayılan konumun genişliğini, grafik alanının kesir birimi cinsinden temsil eder.

```csharp
public double DefaultWidthRatioToChart { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultWidthRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // ChartFrame olan grafik başlığına eriş
            ChartFrame chartTitle = chart.Title;

            // Mevcut DefaultWidthRatioToChart değerini göster
            Console.WriteLine("Current DefaultWidthRatioToChart value: " + chartTitle.DefaultWidthRatioToChart);

            // Not: DefaultWidthRatioToChart sadece okunabilir, bu yüzden ayarlanamaz
            // Bunun yerine, gerçek genişlik oranı ile ilişkisini göstereceğiz
            Console.WriteLine("Current WidthRatioToChart: " + chartTitle.WidthRatioToChart);

            // Genişlik oranını değiştirerek etkisini göster
            chartTitle.WidthRatioToChart = 0.5;
            Console.WriteLine("After setting WidthRatioToChart to 0.5, DefaultWidthRatioToChart remains: " + chartTitle.DefaultWidthRatioToChart);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartFramePropertyDefaultWidthRatioToChartDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


