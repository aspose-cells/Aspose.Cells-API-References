---
title: "Enum FormattingType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.FormattingType enum. Bir Area nesnesine veya Line nesnesine uygulanan biçimlendirme türünü temsil eder."
type: docs
url: /tr/net/aspose.cells.charts/formattingtype/
---
## FormattingType enumeration

Bir [`Area`](../../aspose.cells.drawing/area/) nesnesine veya bir [`Line`](../../aspose.cells.drawing/line/) nesnesine uygulanan biçimlendirme türünü temsil eder.

```csharp
public enum FormattingType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Automatic | `0` | Otomatik biçimlendirme türünü temsil eder. |
| Custom | `2` | Özel biçimlendirme türünü temsil eder. |
| None | `1` | Hiçbir biçimlendirme türünü temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class FormattingTypeDemo
    {
        public static void FormattingTypeExample()
        {
            // Bir Workbook nesnesi oluşturun
            Workbook workbook = new Workbook();
            
            // Workbook nesnesine yeni bir çalışma sayfası ekleme
            int sheetIndex = workbook.Worksheets.Add();
            
            // Eklenen yeni çalışma sayfasının referansını, sayfa indeksini geçirerek elde etme
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Hücrelere örnek değerler ekleme
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            
            // Çalışma sayfasına bir grafik ekleme
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            
            // Yeni eklenen grafiğin örneğine erişme
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafiğe, "A1" hücresinden "B3" hücresine kadar uzanan NSeries (grafik veri kaynağı) ekleniyor
            chart.NSeries.Add("A1:B3", true);
            
            // Grafik alanının ön plan rengini ayarlama
            chart.PlotArea.Area.ForegroundColor = Color.Blue;
            chart.PlotArea.Area.Formatting = FormattingType.Custom;
            
            // Şema alanının ön plan rengini ayarlama
            chart.ChartArea.Area.ForegroundColor = Color.Yellow;
            chart.ChartArea.Area.Formatting = FormattingType.Automatic;
            
            // 1. NSeries alanının ön plan rengini ayarlama
            chart.NSeries[0].Area.ForegroundColor = Color.Red;
            chart.NSeries[0].Area.Formatting = FormattingType.None;
            
            // 1. NSeries noktasının alanının ön plan rengini ayarlama
            chart.NSeries[0].Points[0].Area.ForegroundColor = Color.Cyan;
            chart.NSeries[0].Points[0].Area.Formatting = FormattingType.Custom;
            
            // Excel dosyasını kaydetme
            workbook.Save("FormattingTypeExample.xlsx");
            workbook.Save("FormattingTypeExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


