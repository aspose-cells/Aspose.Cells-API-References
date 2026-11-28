---
title: "TextAlignmentType enum"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.TextAlignmentType enum. Metin hizalama türlerini listeler"
type: docs
url: /tr/net/aspose.cells/textalignmenttype/
---
## TextAlignmentType enumeration

Metin hizalama türlerini listeler.

```csharp
public enum TextAlignmentType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| General | `1792` | Genel metin hizalamasını temsil eder. |
| Bottom | `528` | Alt metin hizalamasını temsil eder. |
| Center | `1802` | Orta metin hizalamasını temsil eder. |
| CenterAcross | `1286` | Ortada yayılmış metin hizalamasını temsil eder. |
| Distributed | `807` | Dağıtılmış metin hizalamasını temsil eder. |
| Fill | `1284` | Doldurma metin hizalamasını temsil eder. |
| Justify | `1821` | İki yana yaslanmış metin hizalamasını temsil eder. |
| Left | `257` | Sol metin hizalamasını temsil eder. |
| Right | `259` | Sağ metin hizalamasını temsil eder. |
| Top | `512` | Üst metin hizalamasını temsil eder. |
| JustifiedLow | `832` | Arapça metin için ayarlanmış kashida uzunluğuyla metni hizalar. |
| ThaiDistributed | `896` | Her karakter bir kelime olarak kabul edildiği için Tayland metnini özel olarak dağıtır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TextAlignmentTypeDemo
    {
        public static void TextAlignmentTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["B4"].PutValue(78);

            // Bir hücreye yorum ekle
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "This is a comment.";
            comment.TextHorizontalAlignment = TextAlignmentType.Center;
            comment.TextVerticalAlignment = TextAlignmentType.Top;

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.SetChartDataRange("A1:B4", true);

            // Grafik başlığını özelleştir
            chart.Title.Text = "Scores Chart";
            chart.Title.TextHorizontalAlignment = TextAlignmentType.Center;
            chart.Title.TextVerticalAlignment = TextAlignmentType.Top;

            // Çalışma kitabını kaydedin
            workbook.Save("TextAlignmentTypeExample.xlsx");

            // Sonuçları çıktı olarak ver.
            Console.WriteLine("Workbook saved successfully with text alignment settings.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


