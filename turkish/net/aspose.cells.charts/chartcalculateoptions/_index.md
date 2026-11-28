---
title: "Sınıf ChartCalculateOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.ChartCalculateOptions sınıfı. Bir grafiğin hesaplanması için seçenekleri temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/chartcalculateoptions/
---
## ChartCalculateOptions class

Bir grafiğin hesaplanması için seçenekleri temsil eder.

```csharp
public class ChartCalculateOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ChartCalculateOptions](chartcalculateoptions/)() | Grafiğin hesaplanması için seçenekleri oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [UpdateAllPoints](../../aspose.cells.charts/chartcalculateoptions/updateallpoints/) { get; set; } | Grafik hesaplaması yapılırken tüm veri noktalarının güncellenip güncellenmeyeceği. Varsayılan: False. Grafikteki her bir veri noktasının değerini özellikle almak istediğinizde, bunu true olarak ayarlayın. Bu parametre True olarak ayarlanırsa, grafik hesaplandığında yeni veri noktaları oluşturulabilir. Bu, Excel dosyasının daha büyük olmasına neden olabilir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCalculateOptionsDemo
    {
        public static void ChartCalculateOptionsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik için veri aralığını ayarlayın
            chart.SetChartDataRange("A1:B4", true);

            // ChartCalculateOptions örneği oluştur
            ChartCalculateOptions options = new ChartCalculateOptions
            {
                UpdateAllPoints = true // Set the property to update all data points
            };

            // Grafiği belirtilen seçeneklerle hesapla
            chart.Calculate(options);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartCalculateOptionsExample.xlsx");
            workbook.Save("ChartCalculateOptionsExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


