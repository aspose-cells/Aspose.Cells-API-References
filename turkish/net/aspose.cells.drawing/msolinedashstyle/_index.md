---
title: "MsoLineDashStyle enum'ı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.MsoLineDashStyle enum'ı. Çizgi çizimindeki tire stilini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/msolinedashstyle/
---
## MsoLineDashStyle enumeration

Kesikli çizgi çizim stilini temsil eder.

```csharp
public enum MsoLineDashStyle
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Dash | `0` | Kesikli bir çizgiyi temsil eder. |
| DashDot | `1` | Kesik noktalı bir çizgi temsil eder. |
| DashDotDot | `2` | Kesikli-nokta-noktalı bir çizgiyi temsil eder. |
| DashLongDash | `3` | Uzun tire-kısa tire çizgisini temsil eder. |
| DashLongDashDot | `4` | Uzun tire-kısa tire-nokta çizgisini temsil eder. |
| RoundDot | `5` | Yuvarlak noktalı bir çizgi temsil eder. |
| Solid | `6` | Düz bir çizgiyi temsil eder. |
| SquareDot | `7` | Kare noktalı bir çizgi temsil eder. |
| Custom | `8` | Özel tire stili. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineDashStyleDemo
    {
        public static void MsoLineDashStyleExample()
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

            // Birincil kategori eksenine eriş
            Axis categoryAxis = chart.CategoryAxis;

            // Ana ızgara çizgilerinin tire stilini ayarla
            categoryAxis.MajorGridLines.DashType = MsoLineDashStyle.DashDot;

            // Alt ızgara çizgilerinin tire stilini ayarla
            categoryAxis.MinorGridLines.DashType = MsoLineDashStyle.DashLongDashDot;

            // Çalışma kitabını kaydedin
            workbook.Save("MsoLineDashStyleExample.xlsx");

            // Sonuçları çıktı olarak ver.
            Console.WriteLine("Chart with custom dash styles for gridlines created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


