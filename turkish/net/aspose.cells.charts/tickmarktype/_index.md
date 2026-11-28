---
title: "TickMarkType enum'ı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.TickMarkType enum. Belirtilen eksen için tik işareti tipini temsil eder."
type: docs
url: /tr/net/aspose.cells.charts/tickmarktype/
---
## TickMarkType enumeration

Belirtilen eksen için işaret işareti türünü temsil eder.

```csharp
public enum TickMarkType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Cross | `0` | Tik işareti tipi Çaprazdır. |
| Inside | `1` | Tik işareti tipi İçeridedir. |
| None | `2` | Tik işareti tipi Yoktur. |
| Outside | `3` | Tik işareti tipi Dışarıdadır |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickMarkTypeDemo
    {
        public static void TickMarkTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
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

            // Grafiğin değer eksenine erişin.
            Axis valueAxis = chart.ValueAxis;

            // Ana tik işareti tipini Çapraz olarak ayarlayın.
            valueAxis.MajorTickMark = TickMarkType.Cross;

            // Küçük tik işareti tipini İçeride olarak ayarlayın.
            valueAxis.MinorTickMark = TickMarkType.Inside;

            // Değer ekseninin maksimum değerini ayarla
            valueAxis.MaxValue = 200;

            // Değer ekseninin minimum değerini ayarla
            valueAxis.MinValue = 0;

            // Ana birimi ayarla
            valueAxis.MajorUnit = 25;

            // Çalışma kitabını kaydedin
            workbook.Save("TickMarkTypeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


