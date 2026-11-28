---
title: "Enum AxisType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.AxisType enum. Eksen tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/axistype/
---
## AxisType enumeration

Eksen tipini temsil eder.

```csharp
public enum AxisType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Category | `0` | Kategori ekseni |
| Value | `1` | Değer ekseni |
| Series | `2` | Seri ekseni |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisTypeDemo
    {
        public static void AxisTypeExample()
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

            // Grafikte hangi eksenlerin mevcut olduğunu belirleyin
            bool hasPrimaryCategoryAxis = chart.HasAxis(AxisType.Category, true);
            bool hasSecondaryCategoryAxis = chart.HasAxis(AxisType.Category, false);
            bool hasPrimaryValueAxis = chart.HasAxis(AxisType.Value, true);
            bool hasSecondaryValueAxis = chart.HasAxis(AxisType.Value, false);

            // Sonuçları çıktı olarak ver.
            Console.WriteLine("Has Primary Category Axis: " + hasPrimaryCategoryAxis);
            Console.WriteLine("Has Secondary Category Axis: " + hasSecondaryCategoryAxis);
            Console.WriteLine("Has Primary Value Axis: " + hasPrimaryValueAxis);
            Console.WriteLine("Has Secondary Value Axis: " + hasSecondaryValueAxis);

            // Çalışma kitabını kaydedin
            workbook.Save("AxisTypeExample.xlsx");
            workbook.Save("AxisTypeExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


