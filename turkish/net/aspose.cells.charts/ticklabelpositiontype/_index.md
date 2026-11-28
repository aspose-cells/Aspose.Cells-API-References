---
title: "Enum TickLabelPositionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.TickLabelPositionType enum. Belirtilen eksende işaret etiketi etiketlerinin konum türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/ticklabelpositiontype/
---
## TickLabelPositionType enumeration

Belirtilen eksende işaret işareti etiketlerinin konum türünü temsil eder.

```csharp
public enum TickLabelPositionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| High | `0` | Konum türü yüksek. |
| Low | `1` | Konum türü düşük. |
| NextToAxis | `2` | Konum türü eksenin yanındadır. |
| None | `3` | Konum türü yok. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickLabelPositionTypeDemo
    {
        public static void TickLabelPositionTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bazı örnek veriler ekleyin
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafiğe "A1" hücresinden "B3" hücresine kadar uzanan NSeries (grafik veri kaynağı) ekleyin
            chart.NSeries.Add("A1:B3", true);
            
            // Kategori eksenine erişin
            Axis categoryAxis = chart.CategoryAxis;
            
            // İşaret etiketi konumunu Yüksek olarak ayarla
            categoryAxis.TickLabelPosition = TickLabelPositionType.High;
            
            // Çalışma kitabını kaydedin
            workbook.Save("TickLabelPositionTypeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


