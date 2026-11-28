---
title: "Axis.BaseUnitScale"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Eksen özelliği. Kategori ekseni için temel birim ölçeğini temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/axis/baseunitscale/
---
## Axis.BaseUnitScale property

Kategori ekseni için temel birim ölçeğini temsil eder.

```csharp
public TimeUnit BaseUnitScale { get; set; }
```

### Açıklamalar

Yalnızca CategoryType özelliği TimeScale olarak ayarlandığında etkili olur.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyBaseUnitScaleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells[$"A{i}"].PutValue(DateTime.Now.AddDays(i));
                sheet.Cells[$"B{i}"].PutValue(i * 100);
            }

            // Bir grafik ekleyin
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Kategori ekseni için temel birim ölçeğini ayarla
            chart.CategoryAxis.BaseUnitScale = TimeUnit.Months;

            // Çalışma kitabını kaydedin
            workbook.Save("AxisPropertyBaseUnitScaleDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TimeUnit](../../timeunit/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


