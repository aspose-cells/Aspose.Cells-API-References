---
title: "Enum MsoArrowheadWidth"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.MsoArrowheadWidth enum. Şekil kenar çizgisinin uç genişliğini sıralar"
type: docs
url: /tr/net/aspose.cells.drawing/msoarrowheadwidth/
---
## MsoArrowheadWidth enumeration

Şekil kenarlık çizgisinin uç genişliğini listeler.

```csharp
public enum MsoArrowheadWidth
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Narrow | `0` | Kısa uç genişliği. |
| Medium | `1` | Orta uç genişliği. |
| Wide | `2` | Geniş uç genişliği. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class MsoArrowheadWidthDemo
    {
        public static void MsoArrowheadWidthExample()
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

            // Grafik için bir çizgi şekli oluşturun
            Line line = chart.Line;

            // Ok ucu stillerini ve genişliklerini ayarlayın
            line.BeginType = MsoArrowheadStyle.Arrow;
            line.BeginArrowWidth = MsoArrowheadWidth.Wide;
            line.EndType = MsoArrowheadStyle.Arrow;
            line.EndArrowWidth = MsoArrowheadWidth.Narrow;

            // Ok ucu stillerini ve genişliklerini çıktı olarak verin
            Console.WriteLine("Begin Arrowhead Width: " + line.BeginArrowWidth);
            Console.WriteLine("End Arrowhead Width: " + line.EndArrowWidth);

            // Çalışma kitabını kaydedin
            workbook.Save("MsoArrowheadWidthExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


