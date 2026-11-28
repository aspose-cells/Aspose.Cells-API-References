---
title: "Enum Bar3DShapeType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.Bar3DShapeType enum. 3D çubuk veya sütun grafiğinde kullanılan şekli temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/bar3dshapetype/
---
## Bar3DShapeType enumeration

3D çubuk veya sütun grafiğiyle kullanılan şekli temsil eder.

```csharp
public enum Bar3DShapeType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Box | `0` | Kutu |
| PyramidToPoint | `1` | PyramidToPoint |
| PyramidToMax | `2` | PyramidToMax |
| Cylinder | `3` | Cylinder |
| ConeToPoint | `4` | ConeToPoint |
| ConeToMax | `5` | ConeToMax |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class Bar3DShapeTypeDemo
    {
        public static void Bar3DShapeTypeExample()
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
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Çalışma sayfasına bir grafik ekleme
            int chartIndex = worksheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 15, 5);
            // Yeni eklenen grafiğin örneğine erişme
            Chart chart = worksheet.Charts[chartIndex];
            // Grafiğe, "A1" hücresinden "B4" hücresine kadar olan NSeries (grafik veri kaynağı) ekleme.
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            // NSeries'in kategori verileri için veri kaynağını ayarlama
            chart.NSeries.CategoryData = "C1:C4";
            Series series = chart.NSeries[seriesIndex];
            // Serinin değerlerini ayarlama
            series.Values = "=B1:B4";

            // Seri için 3B şekil tipini ayarlama
            series.Bar3DShapeType = Bar3DShapeType.Cylinder;

            // Excel dosyasını kaydetme
            workbook.Save("Bar3DShapeTypeExample.xlsx");
            workbook.Save("Bar3DShapeTypeExample.pdf");

            // Seri için 3B şekil tipini ayarlama
            series.Bar3DShapeType = Bar3DShapeType.ConeToMax;

            // Excel dosyasını kaydetme
            workbook.Save("Bar3DShapeTypeExample2.xlsx");
            workbook.Save("Bar3DShapeTypeExample2.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


