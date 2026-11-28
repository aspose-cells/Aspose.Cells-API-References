---
title: "Enum CategoryType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.CategoryType enum. Kategori eksen tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/categorytype/
---
## CategoryType enumeration

Kategori eksen tipini temsil eder.

```csharp
public enum CategoryType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| AutomaticScale | `0` | AutomaticScale |
| CategoryScale | `1` | CategoryScale |
| TimeScale | `2` | TimeScale |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class CategoryTypeDemo
    {
        public static void CategoryTypeExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();
            // Excel nesnesine yeni bir çalışma sayfası ekleme
            int sheetIndex = workbook.Worksheets.Add();
            // Eklenen yeni çalışma sayfasının referansını, sayfa indeksini geçirerek elde etme
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Hücrelere örnek değerler ekleme
            worksheet.Cells["A1"].PutValue("Dates");
            worksheet.Cells["A2"].PutValue(new DateOnly(2024, 01, 01));
            worksheet.Cells["A3"].PutValue(new DateOnly(2024, 03, 01));
            worksheet.Cells["A4"].PutValue(new DateOnly(2024, 05, 01));
            worksheet.Cells["B1"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Data2");
            worksheet.Cells["C2"].PutValue(8);
            worksheet.Cells["C3"].PutValue(15);
            worksheet.Cells["C4"].PutValue(30);

            // Çalışma sayfasına bir grafik ekleme
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            // Yeni eklenen grafiğin örneğine erişme
            Chart chart = worksheet.Charts[chartIndex];
            // Grafiğe, "A1" hücresinden "B3" hücresine kadar uzanan NSeries (grafik veri kaynağı) ekleniyor
            chart.NSeries.Add("B2:C4", true);

            // X-ekseninin kategori adlarını "A2:A5" aralığından ayarlama
            chart.NSeries[0].XValues = "A2:A4";

            // Kategori eksen tipini TimeScale olarak ayarlama
            chart.CategoryAxis.CategoryType = CategoryType.CategoryScale;

            // Kategori ekseni için ana birim ölçeğini ayarlama
            chart.CategoryAxis.MajorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MajorUnit = 2;

            // Kategori ekseni için alt birim ölçeğini ayarlama
            chart.CategoryAxis.MinorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MinorUnit = 2;

            // Excel dosyasını kaydetme
            workbook.Save("CategoryTypeExample.xlsx");
            workbook.Save("CategoryTypeExample.pdf");

        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


