---
title: "Axis.MajorTickMark"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Axis özelliği. Belirtilen eksen için ana işaretçenin tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/axis/majortickmark/
---
## Axis.MajorTickMark property

Belirtilen eksen için ana tik işaretinin tipini temsil eder.

```csharp
public TickMarkType MajorTickMark { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMajorTickMarkDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Bir sütun grafik ekle
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ana işaretçi tipini dışa ayarla
            chart.ValueAxis.MajorTickMark = TickMarkType.Outside;

            // Çalışma kitabını kaydedin
            workbook.Save("AxisPropertyMajorTickMarkDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TickMarkType](../../tickmarktype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


