---
title: "Enum TickLabelAlignmentType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.TickLabelAlignmentType enum. Eksende tik etiketlerinin metin hizalama türünü temsil eder."
type: docs
url: /tr/net/aspose.cells.charts/ticklabelalignmenttype/
---
## TickLabelAlignmentType enumeration

Eksen üzerindeki işaret etiketi metin hizalama türünü temsil eder

```csharp
public enum TickLabelAlignmentType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Center | `0` | Metnin ortalandığını belirtir. |
| Left | `1` | Metnin sola hizalandığını belirtir. |
| Right | `2` | Metnin sağa hizalanacağını belirtir.. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickLabelAlignmentTypeDemo
    {
        public static void TickLabelAlignmentTypeExample()
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

            // Grafiğe seri ekle
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Kategori ekseninin işaret etiketlerine erişin
            TickLabels tickLabels = chart.CategoryAxis.TickLabels;

            // İşaret etiketleri için hizalama tipini ayarla
            tickLabels.AlignmentType = TickLabelAlignmentType.Center;

            // Çalışma kitabını kaydedin
            workbook.Save("TickLabelAlignmentTypeExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


