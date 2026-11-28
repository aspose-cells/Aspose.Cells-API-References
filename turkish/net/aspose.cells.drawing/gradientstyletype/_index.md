---
title: "Enum GradientStyleType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.GradientStyleType enum. Gradyan gölgelendirme stilini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/gradientstyletype/
---
## GradientStyleType enumeration

Degrade gölgelendirme stilini temsil eder.

```csharp
public enum GradientStyleType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| DiagonalDown | `0` | Diyagonal aşağı gölgelendirme stili |
| DiagonalUp | `1` | Diyagonal yukarı gölgelendirme stili |
| FromCenter | `2` | Merkezden gölgelendirme stili |
| FromCorner | `3` | Köşeden gölgelendirme stili |
| Horizontal | `4` | Yatay gölgelendirme stili |
| Vertical | `5` | Dikey gölgelendirme stili |
| Unknown | `6` | Bilinmeyen gölgelendirme stili. Şablon dosyasındaki GradientStyleType üyesi olmayan gölgelendirme stili için yalnızca. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStyleTypeDemo
    {
        public static void GradientStyleTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
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

            // Grafik veri aralığını ayarla
            chart.SetChartDataRange("A1:B4", true);

            // Grafiğin çizim alanına erişin
            PlotArea plotArea = chart.PlotArea;

            // Çizim alanının doldurma biçimine erişin
            FillFormat fillFormat = plotArea.Area.FillFormat;

            // DiagonalDown stilinde iki renkli bir gradyan doldurma ayarlayın
            fillFormat.SetTwoColorGradient(Color.Blue, Color.White, GradientStyleType.DiagonalDown, 1);

            // Kullanılan gradyan stilini çıktı olarak ver
            Console.WriteLine("Gradient Style: " + fillFormat.GradientStyle);

            // Çalışma kitabını kaydedin
            workbook.Save("GradientStyleTypeExample.xlsx");
            workbook.Save("GradientStyleTypeExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


