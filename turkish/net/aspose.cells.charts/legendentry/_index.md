---
title: "Sınıf LegendEntry"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.LegendEntry sınıfı. Bir grafik açıklamasındaki bir legend girişini temsil eder."
type: docs
url: /tr/net/aspose.cells.charts/legendentry/
---
## LegendEntry class

Grafik açıklamasındaki bir açıklama girişini temsil eder.

```csharp
public class LegendEntry
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AutoScaleFont](../../aspose.cells.charts/legendentry/autoscalefont/) { get; set; } | Nesnedeki metin, nesne boyutu değiştiğinde yazı tipi boyutunu değiştiriyorsa True döner. Varsayılan değer True'dur. |
| [Background](../../aspose.cells.charts/legendentry/background/) { get; set; } | (**Obsolete.**) Arka planın görüntüleme modunu alır ve ayarlar |
| [BackgroundMode](../../aspose.cells.charts/legendentry/backgroundmode/) { get; set; } | Arka planın görüntüleme modunu alır ve ayarlar |
| [Font](../../aspose.cells.charts/legendentry/font/) { get; } | Belirtilen ChartFrame nesnesinin bir [`Font`](./font/) nesnesini alır. |
| [IsDeleted](../../aspose.cells.charts/legendentry/isdeleted/) { get; set; } | Legend girişinin silinip silinmediğini alır ve ayarlar. |
| [IsTextNoFill](../../aspose.cells.charts/legendentry/istextnofill/) { get; set; } | Metnin doldurulmasını alır veya ayarlar. |
| virtual [TextFont](../../aspose.cells.charts/legendentry/textfont/) { get; } | (**Obsolete.**) Belirtilen LegendEntry nesnesinin bir [`Font`](./font/) nesnesini alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendEntryDemo
    {
        public static void LegendEntryExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafiğe, "A1" hücresinden "B4" hücresine kadar olan NSeries (grafik veri kaynağı) ekle.
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // İlk serinin açıklama girişine erişin.
            LegendEntry legendEntry = chart.NSeries[0].LegendEntry;

            // Açıklama girişinin özelliklerini ayarlayın.
            legendEntry.IsDeleted = false;
            legendEntry.IsTextNoFill = false;
            legendEntry.AutoScaleFont = true;
            legendEntry.Background = BackgroundMode.Transparent;
            legendEntry.BackgroundMode = BackgroundMode.Opaque;

            // Açıklama girişinin yazı tipine erişin ve değiştirin.
            Font font = legendEntry.Font;
            font.Name = "Arial";
            font.Size = 12;
            font.IsBold = true;
            font.Color = System.Drawing.Color.Blue;

            // Çalışma kitabını kaydedin
            workbook.Save("LegendEntryExample.xlsx");
            workbook.Save("LegendEntryExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


