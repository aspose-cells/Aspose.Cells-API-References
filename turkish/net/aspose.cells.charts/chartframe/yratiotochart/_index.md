---
title: "ChartFrame.YRatioToChart"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartFrame özelliği. Grafik alanının oran biriminde sol üst köşenin y koordinatını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/chartframe/yratiotochart/
---
## ChartFrame.YRatioToChart property

Üst sol köşenin y koordinatını, çizelge alanının oran biriminde alır veya ayarlar.

```csharp
public virtual double YRatioToChart { get; set; }
```

### Açıklamalar

Bu bir kesir değeridir, geçerli aralığı 0-1 arasındadır. Oran birimlerini piksellere nasıl dönüştürülür? YPixel = YRatioToChart * Chart.ChartObject.Height;

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyYRatioToChartDemo
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
            
            // ChartFrame'den miras alan grafik başlığına erişin
            chart.Title.Text = "Sample Chart";
            
            // Mevcut YRatioToChart değerini göster
            Console.WriteLine("Current Title YRatioToChart value: " + chart.Title.YRatioToChart);
            
            // Başlığın grafik alanına göre Y konumunu değiştir
            chart.Title.YRatioToChart = 0.1; // 10% from top of chart area
            
            // Yeni YRatioToChart değerini göster
            Console.WriteLine("New Title YRatioToChart value: " + chart.Title.YRatioToChart);
            
            // ChartFrame'den de miras alan lejanta eriş
            chart.Legend.Position = LegendPositionType.Top;
            
            // Lejant için mevcut YRatioToChart değerini göster
            Console.WriteLine("Current Legend YRatioToChart value: " + chart.Legend.YRatioToChart);
            
            // Lejantın grafik alanına göre Y konumunu değiştir
            chart.Legend.YRatioToChart = 0.15; // 15% from top of chart area
            
            // Lejant için yeni YRatioToChart değerini göster
            Console.WriteLine("New Legend YRatioToChart value: " + chart.Legend.YRatioToChart);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ChartFramePropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


