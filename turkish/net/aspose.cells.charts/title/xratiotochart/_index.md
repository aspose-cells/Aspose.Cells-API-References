---
title: "Title.XRatioToChart"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Title özelliği. Grafik alanının kesir biriminde sol üst köşenin x koordinatını alır veya ayarlar. X Pikselde  XRatioToChart  Chart.ChartObject.Width"
type: docs
url: /tr/net/aspose.cells.charts/title/xratiotochart/
---
## Title.XRatioToChart property

Üst sol köşenin x koordinatını, grafik alanının kesir birimi cinsinden alır veya ayarlar. X Piksel = XRatioToChart * Chart.ChartObject.Width;

```csharp
public override double XRatioToChart { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TitlePropertyXRatioToChartDemo
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

            // Grafik için veri kaynağını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafik başlığını al
            chart.Title.Text = "Sample Chart Title";
            Title title = chart.Title;

            // Mevcut XRatioToChart değerini göster
            Console.WriteLine("Current XRatioToChart value: " + title.XRatioToChart);

            // Başlığı yatay olarak hareket ettirmek için XRatioToChart değerini değiştir
            title.XRatioToChart = 0.25; // 25% from the left of the chart area
            Console.WriteLine("New XRatioToChart value: " + title.XRatioToChart);

            // Çalışma kitabını kaydedin
            workbook.Save("TitlePropertyXRatioToChartDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


