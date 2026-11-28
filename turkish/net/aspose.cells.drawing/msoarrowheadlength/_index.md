---
title: "MsoArrowheadLength enumı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.MsoArrowheadLength enumı. Şekil kenar çizgisinin uç genişliğini sıralar"
type: docs
url: /tr/net/aspose.cells.drawing/msoarrowheadlength/
---
## MsoArrowheadLength enumeration

Şekil kenarlık çizgisinin uç genişliğini listeler.

```csharp
public enum MsoArrowheadLength
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Short | `0` | Kısa çizgi ucu uzunluğu |
| Medium | `1` | Orta çizgi ucu uzunluğu |
| Long | `2` | Uzun çizgi ucu uzunluğu |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoArrowheadLengthDemo
    {
        public static void MsoArrowheadLengthExample()
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
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.SetChartDataRange("A1:B4", true);

            // Grafik için bir çizgi şekli oluşturun
            Line line = chart.Line;

            // Ok başı uzunluklarını ayarlayın
            line.BeginArrowLength = MsoArrowheadLength.Medium;
            line.EndArrowLength = MsoArrowheadLength.Long;

            // Ok ucu uzunluklarını çıktı olarak ver
            Console.WriteLine("Begin Arrowhead Length: " + line.BeginArrowLength);
            Console.WriteLine("End Arrowhead Length: " + line.EndArrowLength);

            // Çalışma kitabını kaydedin
            workbook.Save("MsoArrowheadLengthExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


