---
title: "Sınıf Area"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Area sınıfı. Bir alan biçimini temsil eden nesneyi kapsüller"
type: docs
url: /tr/net/aspose.cells.drawing/area/
---
## Area class

Bir alan biçimini temsil eden nesneyi kapsüller.

```csharp
public class Area
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | `Area` nesnesinin arka plan Rengini alır veya ayarlar. |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Belirtilen grafik veya şekil için doldurma biçim özelliklerini içeren bir [`FillFormat`](./fillformat/) nesnesini temsil eder. |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Ön plan rengini alır veya ayarlar. |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Alan biçimini temsil eder. |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | Özellik true ise ve grafik noktasının değeri negatif bir sayı ise, ön plan rengi ve arka plan rengi değiştirilecektir. |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Alan şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak döndürür veya ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class AreaDemo
    {
        public static void AreaExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();
            // Workbook nesnesine yeni bir çalışma sayfası ekleme
            int sheetIndex = workbook.Worksheets.Add();
            // Eklenen yeni çalışma sayfasının referansını, sayfa indeksini geçirerek elde etme
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Hücrelere örnek değerler ekleme
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(-100);
            worksheet.Cells["A3"].PutValue(150);
            // Çalışma sayfasına bir grafik ekleme
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 15, 5);
            // Yeni eklenen grafiğin örneğine erişme
            Chart chart = worksheet.Charts[chartIndex];
            // "A1" hücresinden "A3" hücresine kadar olan aralıkta grafiğe NSeries (grafik veri kaynağı) ekleniyor
            chart.NSeries.Add("A1:A3", true);

            // İlk NSeries'in alanına erişiliyor
            Area area = chart.NSeries[0].Area;

            // Özellikleri ayarlama
            area.InvertIfNegative = true;
            area.ForegroundColor = Color.Red;
            area.BackgroundColor = Color.Yellow;
            area.Formatting = Aspose.Cells.Charts.FormattingType.Custom;
            area.Transparency = 0.5;

            // Excel dosyasını kaydetme
            workbook.Save("AreaExample.xlsx");
            workbook.Save("AreaExample.pdf");

        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


