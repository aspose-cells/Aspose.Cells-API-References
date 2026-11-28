---
title: "Enum LineType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.LineType enum. Resim kenarlığı veya Grafik çizgisinin türünü sıralar"
type: docs
url: /tr/net/aspose.cells.drawing/linetype/
---
## LineType enumeration

Resim kenarlığının [`Picture`](../picture/) veya [`Chart`](../../aspose.cells.charts/chart/) çizgisinin türünü sıralar.

```csharp
public enum LineType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| DarkGray | `6` | Koyu gri bir çizgiyi temsil eder. |
| Dash | `1` | Kesikli bir çizgiyi temsil eder. |
| DashDot | `3` | Kesikli-noktalı bir çizgiyi temsil eder |
| DashDotDot | `4` | Kesikli-nokta-noktalı bir çizgiyi temsil eder. |
| Dot | `2` | Noktalı bir çizgiyi temsil eder. |
| LightGray | `8` | Açık gri bir çizgiyi temsil eder. |
| MediumGray | `7` | Orta gri bir çizgiyi temsil eder. |
| Solid | `0` | Düz bir çizgiyi temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class LineTypeDemo
    {
        public static void LineTypeExample()
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

            // Eksen çizgisi için çizgi tipini ayarla
            categoryAxis.AxisLine.Style = LineType.DashDot;

            // Eksen çizgisinin rengini ayarla
            categoryAxis.AxisLine.Color = Color.Blue;

            // Birincil değer eksenine erişin
            Axis valueAxis = chart.ValueAxis;

            // Ana ızgara çizgileri için çizgi tipini ayarla
            valueAxis.MajorGridLines.Style = LineType.Dot;

            // Ana ızgara çizgilerinin rengini ayarla
            valueAxis.MajorGridLines.Color = Color.Red;

            // Çalışma kitabını kaydedin
            workbook.Save("LineTypeExample.xlsx");

            // Sonuçları çıktı olarak ver.
            Console.WriteLine("Chart created with custom line types for axis and gridlines.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


