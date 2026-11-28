---
title: "Enum LineJoinType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.LineJoinType enum. Bir çizginin birleşim stillerini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/linejointype/
---
## LineJoinType enumeration

Bir çizginin birleşim stillerini temsil eder.

```csharp
public enum LineJoinType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Round | `0` | Yuvarlak eklem |
| Bevel | `1` | Koni eklem |
| Miter | `2` | Köşe eklem |
| None | `3` | Eklem yok |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class LineJoinTypeDemo
    {
        public static void LineJoinTypeExample()
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

            // Birincil değer eksenine erişin
            Axis valueAxis = chart.ValueAxis;

            // Ana ızgara çizgilerinin çizgi biçimine erişin
            Line majorGridLines = valueAxis.MajorGridLines;

            // Çizginin eklem tipini ayarlayın
            majorGridLines.JoinType = LineJoinType.Round;

            // Eklem tipini çıktı olarak verin
            Console.WriteLine("Line Join Type: " + majorGridLines.JoinType);

            // Çalışma kitabını kaydedin
            workbook.Save("LineJoinTypeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


