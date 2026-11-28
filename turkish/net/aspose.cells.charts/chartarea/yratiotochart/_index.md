---
title: "ChartArea.YRatioToChart"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartArea özelliği. Grafik alanının üst sol köşe satırından dikey ofseti, grafik alanının oran biriminde alır veya alır."
type: docs
url: /tr/net/aspose.cells.charts/chartarea/yratiotochart/
---
## ChartArea.YRatioToChart property

Grafik alanının üst sol köşe satırından dikey ofseti alır veya alır, grafik alanının oran birimi olarak.

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

    public class ChartAreaPropertyYRatioToChartDemo
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
            
            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafik alanına eriş
            ChartArea chartArea = chart.ChartArea;

            // Mevcut YRatioToChart değerini göster
            Console.WriteLine("Current YRatioToChart value: " + chartArea.YRatioToChart);

            // YRatioToChart özelliğini değiştir (0.0 ile 1.0 arasında, grafik alanının %0 ile %100'ünü temsil eder)
            chartArea.YRatioToChart = 0.2; // Move chart area down by 20% of chart height

            // Yeni YRatioToChart değerini göster
            Console.WriteLine("New YRatioToChart value: " + chartArea.YRatioToChart);

            // Etkiyi görmek için çalışma kitabını kaydet
            workbook.Save("ChartAreaPropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


