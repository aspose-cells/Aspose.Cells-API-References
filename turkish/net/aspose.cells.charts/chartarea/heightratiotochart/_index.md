---
title: "ChartArea.HeightRatioToChart"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartArea özelliği. Grafik alanının alt sağ köşe satırından dikey ofseti, grafik alanının oran biriminde alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/chartarea/heightratiotochart/
---
## ChartArea.HeightRatioToChart property

Grafik alanının alt sağ köşe satırından dikey ofseti alır veya ayarlar, grafik alanının oran birimi olarak.

```csharp
public override double HeightRatioToChart { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartAreaPropertyHeightRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Grafik alanına eriş
            ChartArea chartArea = chart.ChartArea;

            // Mevcut HeightRatioToChart değerini göster
            Console.WriteLine("Current HeightRatioToChart value: " + chartArea.HeightRatioToChart);

            // HeightRatioToChart için yeni bir değer ayarla (0.5 = grafiğin yüksekliğinin %50'si)
            chartArea.HeightRatioToChart = 0.5;
            Console.WriteLine("New HeightRatioToChart value: " + chartArea.HeightRatioToChart);

            // Birleşik etkiyi göstermek için WidthRatioToChart için yeni bir değer ayarla
            chartArea.WidthRatioToChart = 0.8;

            // Değişiklikleri görmek için çalışma kitabını kaydedin
            workbook.Save("ChartAreaPropertyHeightRatioToChartDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


