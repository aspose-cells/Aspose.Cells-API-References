---
title: "Sınıf TickLabels"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.TickLabels sınıfı. Bir grafik eksenindeki işaretçi etiketlerini temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/ticklabels/
---
## TickLabels class

Grafik eksenindeki işaret çizgileriyle ilişkili işaret çizgisi etiketlerini temsil eder.

```csharp
public class TickLabels
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AlignmentType](../../aspose.cells.charts/ticklabels/alignmenttype/) { get; set; } | Eksen üzerindeki işaretçi etiketleri için metin hizalamasını alır ve ayarlar. |
| [AutoScaleFont](../../aspose.cells.charts/ticklabels/autoscalefont/) { get; set; } | Nesnedeki metin, nesne boyutu değiştiğinde yazı tipi boyutunu değiştiriyorsa True döner. Varsayılan değer True'dur. |
| [BackgroundMode](../../aspose.cells.charts/ticklabels/backgroundmode/) { get; set; } | Arka planın görüntüleme modunu alır ve ayarlar |
| [DirectionType](../../aspose.cells.charts/ticklabels/directiontype/) { get; set; } | Metnin yönünü alır ve ayarlar. |
| [DisplayNumberFormat](../../aspose.cells.charts/ticklabels/displaynumberformat/) { get; } | İşaretçi etiketlerinin görüntüleme sayı biçimini alır ve ayarlar. |
| [Font](../../aspose.cells.charts/ticklabels/font/) { get; } | Belirtilen TickLabels nesnesinin yazı tipini temsil eden bir [`Font`](./font/) nesnesi döndürür. |
| [IsAutomaticRotation](../../aspose.cells.charts/ticklabels/isautomaticrotation/) { get; set; } | Dönüş açısının otomatik olup olmadığını gösterir |
| [Number](../../aspose.cells.charts/ticklabels/number/) { get; set; } | TickLabels nesnesi için biçim numarasını temsil eder. |
| [NumberFormat](../../aspose.cells.charts/ticklabels/numberformat/) { get; set; } | TickLabels nesnesi için biçim dizesini temsil eder. |
| [NumberFormatLinked](../../aspose.cells.charts/ticklabels/numberformatlinked/) { get; set; } | Sayı biçimi hücrelere bağlıysa doğru (bu sayede hücrelerde değiştiğinde etiketlerdeki sayı biçimi de değişir). |
| [Offset](../../aspose.cells.charts/ticklabels/offset/) { get; set; } | Etiketlerin kategori ekseninden (x) uzaklığını alır ve ayarlar. Bu yalnızca kategori (x) ekseni için geçerlidir. |
| [ReadingOrder](../../aspose.cells.charts/ticklabels/readingorder/) { get; set; } | Metin okuma sırasını temsil eder. |
| [RotationAngle](../../aspose.cells.charts/ticklabels/rotationangle/) { get; set; } | Metin dönüş açısını saat yönünde temsil eder. |
| [TextDirection](../../aspose.cells.charts/ticklabels/textdirection/) { get; set; } | (**Obsolete.**) Metin okuma sırasını temsil eder. |
| [TickLabelItems](../../aspose.cells.charts/ticklabels/ticklabelitems/) { get; } | Eksenin görüntülenen işaret etiketlerini alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickLabelsDemo
    {
        public static void TickLabelsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
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

            // Değer eksenine erişin
            Axis valueAxis = chart.ValueAxis;

            // Değer ekseninin işaret etiketlerine erişin
            TickLabels tickLabels = valueAxis.TickLabels;

            // İşaret etiketlerinin özelliklerini ayarlayın
            tickLabels.AutoScaleFont = true;
            tickLabels.BackgroundMode = BackgroundMode.Transparent;
            tickLabels.RotationAngle = 45;
            tickLabels.IsAutomaticRotation = false;
            tickLabels.NumberFormat = "0.00";
            tickLabels.Number = 2;
            tickLabels.NumberFormatLinked = true;
            tickLabels.Offset = 100;
            tickLabels.TextDirection = TextDirectionType.LeftToRight;
            tickLabels.ReadingOrder = TextDirectionType.LeftToRight;
            tickLabels.DirectionType = ChartTextDirectionType.Horizontal;
            tickLabels.AlignmentType = TickLabelAlignmentType.Center;

            // Çalışma kitabını kaydedin
            workbook.Save("TickLabelsExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


