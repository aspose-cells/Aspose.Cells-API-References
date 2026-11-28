---
title: "Enum LabelPositionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.LabelPositionType enum. Veri etiketi konum tipi temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/labelpositiontype/
---
## LabelPositionType enumeration

Veri etiketi konum türünü temsil eder.

```csharp
public enum LabelPositionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Center | `0` | Yalnızca çubuk, 2D/3D pasta grafiklerine uygulanır |
| InsideBase | `1` | Yalnızca çubuk, 2D/3D pasta grafiklerine uygulanır |
| InsideEnd | `2` | Yalnızca çubuk grafiklerine uygulanır |
| OutsideEnd | `3` | Yalnızca çubuk, 2d/3d pasta grafiklerine uygulanır |
| Above | `4` | Yalnızca çizgi grafiklerine uygulanır |
| Below | `5` | Yalnızca çizgi grafiklerine uygulanır |
| Left | `6` | Yalnızca çizgi grafiklerine uygulanır |
| Right | `7` | Yalnızca çizgi grafiklerine uygulanır |
| BestFit | `8` | Yalnızca 2D/3D pasta grafiklerine uygulanır |
| Moved | `9` | Kullanıcı veri etiketlerini taşıdı. Bu yalnızca şablon dosyasından grafiği okuma içindir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LabelPositionTypeDemo
    {
        public static void LabelPositionTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için bazı örnek veriler ekleyin
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

            // Veri serisini grafiğe ekle
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // İlk serinin veri etiketlerine eriş
            DataLabels dataLabels = chart.NSeries[0].DataLabels;

            // Veri etiketlerinin konumunu ayarla
            dataLabels.Position = LabelPositionType.InsideBase;

            // Veri etiketlerinde kategori adını göster
            dataLabels.ShowCategoryName = true;

            // Veri etiketlerinde değeri göster
            dataLabels.ShowValue = true;

            // Çalışma kitabını kaydedin
            workbook.Save("LabelPositionTypeExample.xlsx");
            workbook.Save("LabelPositionTypeExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


