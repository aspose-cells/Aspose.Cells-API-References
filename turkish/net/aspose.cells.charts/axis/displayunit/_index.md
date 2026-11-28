---
title: "Axis.DisplayUnit"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Axis özelliği. Belirtilen eksen için birim etiketini temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/axis/displayunit/
---
## Axis.DisplayUnit property

Belirtilen eksen için birim etiketini temsil eder.

```csharp
public DisplayUnitType DisplayUnit { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyDisplayUnitDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10000);
            worksheet.Cells["B3"].PutValue(20000);
            worksheet.Cells["B4"].PutValue(30000);

            // Bir sütun grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Değer ekseni için birim etiketini binlere ayarla
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;

            // Çalışma kitabını kaydedin
            workbook.Save("AxisPropertyDisplayUnitDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* enum [DisplayUnitType](../../displayunittype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


