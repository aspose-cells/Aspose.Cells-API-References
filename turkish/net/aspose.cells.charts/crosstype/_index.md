---
title: "Enum CrossType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.CrossType enum. Eksen kesişim türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/crosstype/
---
## CrossType enumeration

Eksen kesişim tipini temsil eder.

```csharp
public enum CrossType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Automatic | `0` | Microsoft Excel eksen kesişim noktasını ayarlar. |
| Maximum | `1` | Eksen maksimum değerde kesişir. |
| Minimum | `2` | Eksen, minimum değerde kesişir. |
| Custom | `3` | Eksen, özel değerde kesişir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class CrossTypeDemo
    {
        public static void CrossTypeExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();
            // Excel nesnesine yeni bir çalışma sayfası ekleme
            int sheetIndex = workbook.Worksheets.Add();
            // Eklenen yeni çalışma sayfasının referansını, sayfa indeksini geçirerek elde etme
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Hücrelere örnek değerler ekleme
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Çalışma sayfasına bir grafik ekleme
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            // Yeni eklenen grafiğin örneğine erişme
            Chart chart = worksheet.Charts[chartIndex];
            // Grafiğe, "A1" hücresinden "B3" hücresine kadar uzanan NSeries (grafik veri kaynağı) ekleniyor
            chart.NSeries.Add("A1:B3", true);

            // Değer ekseninin maksimum değerini ayarla
            chart.ValueAxis.MaxValue = 200;
            // Değer ekseninin minimum değerini ayarla
            chart.ValueAxis.MinValue = 0;
            // Ana birimi ayarla
            chart.ValueAxis.MajorUnit = 25;

            // Category(X) ekseni, maksimum değerde kesişir
            chart.ValueAxis.CrossType = CrossType.Maximum;

            // Tik işareti etiketleri arasındaki kategori veya seri sayısını ayarla
            chart.CategoryAxis.TickLabelSpacing = 2;

            // Excel dosyasını kaydetme
            workbook.Save("CrossTypeExample.xlsx");
            workbook.Save("CrossTypeExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


