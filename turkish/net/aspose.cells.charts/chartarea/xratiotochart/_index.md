---
title: "ChartArea.XRatioToChart"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartArea özelliği. Grafik alanının sol üst köşe sütunundan yatay offseti, grafik alanının oranı olarak alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/chartarea/xratiotochart/
---
## ChartArea.XRatioToChart property

Grafik alanının üst‑sol köşe sütunundan yatay ofseti alır veya ayarlar, grafik alanının oranı olarak.

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

    public class ChartAreaPropertyXRatioToChartDemo
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

            // Grafik alanını alın
            ChartArea chartArea = chart.ChartArea;

            // Mevcut XRatioToChart değerini gösterin
            Console.WriteLine("Current XRatioToChart value: " + chartArea.XRatioToChart);

            // Grafik alanını yatay olarak taşımak için XRatioToChart değerini değiştirin
            chartArea.XRatioToChart = 0.2; // 20% from the left of the chart container

            // Yeni XRatioToChart değerini gösterin
            Console.WriteLine("New XRatioToChart value: " + chartArea.XRatioToChart);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartAreaXRatioToChartDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


