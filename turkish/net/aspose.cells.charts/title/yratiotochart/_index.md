---
title: "Title.YRatioToChart"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Title özelliği. Grafik alanının kesir biriminde sol üst köşenin y koordinatını alır veya ayarlar. Y Pikselde  YRatioToChart  Chart.ChartObject.Width"
type: docs
url: /tr/net/aspose.cells.charts/title/yratiotochart/
---
## Title.YRatioToChart property

Üst sol köşenin y koordinatını, grafik alanının kesir birimi cinsinden alır veya ayarlar. Y Piksel = YRatioToChart * Chart.ChartObject.Width;

```csharp
public override double YRatioToChart { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TitlePropertyYRatioToChartDemo
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

            // Grafik başlığını al
            chart.Title.Text = "Sample Chart Title";
            Title chartTitle = chart.Title;

            // Mevcut YRatioToChart değerini göster
            Console.WriteLine("Current YRatioToChart value: " + chartTitle.YRatioToChart);

            // Başlığı dikey olarak taşımak için YRatioToChart özelliğini değiştir
            chartTitle.YRatioToChart = 0.1; // 10% from the top of the chart area
            Console.WriteLine("New YRatioToChart value: " + chartTitle.YRatioToChart);

            // Çalışma kitabını kaydedin
            workbook.Save("TitlePropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


