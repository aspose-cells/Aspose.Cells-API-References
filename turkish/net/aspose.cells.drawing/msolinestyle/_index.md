---
title: "Enum MsoLineStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.MsoLineStyle enum. Çizgi çizme stilini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/msolinestyle/
---
## MsoLineStyle enumeration

Çizgi çizim stilini temsil eder.

```csharp
public enum MsoLineStyle
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Single | `0` | Tek çizgi (lineWidth genişliğinde) |
| ThickBetweenThin | `1` | Üç çizgi, ince, kalın, ince |
| ThinThick | `2` | Çift çizgi, biri ince, biri kalın |
| ThickThin | `3` | Çift çizgi, biri kalın, biri ince |
| ThinThin | `4` | Eşit genişlikte çift çizgi |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineStyleDemo
    {
        public static void MsoLineStyleExample()
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

            // Birincil kategori ekseni için çizgi stilini ayarla
            Line axisLine = categoryAxis.AxisLine;
            axisLine.CompoundType = MsoLineStyle.ThickBetweenThin;
            axisLine.Color = Color.Blue;
            axisLine.WeightPt = 2.0;

            // Çizgi stilini çıktı olarak ver
            Console.WriteLine("Axis Line Style: " + axisLine.CompoundType);
            Console.WriteLine("Axis Line Color: " + axisLine.Color);
            Console.WriteLine("Axis Line Weight: " + axisLine.WeightPt);

            // Çalışma kitabını kaydedin
            workbook.Save("MsoLineStyleExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


