---
title: "Axis.MajorUnitScale"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Axis özelliği. Kategori ekseni için ana birim ölçeğini temsil eder."
type: docs
url: /tr/net/aspose.cells.charts/axis/majorunitscale/
---
## Axis.MajorUnitScale property

Kategori ekseni için ana birim ölçeğini temsil eder.

```csharp
public TimeUnit MajorUnitScale { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMajorUnitScaleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek zaman ölçeği verisi ekle
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 5, 1));
            worksheet.Cells["B4"].PutValue(30);
            
            // Grafik oluştur
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);
            
            // Kategori eksenini her 2 ayda bir ana birim olacak şekilde zaman ölçeği olarak yapılandır
            chart.CategoryAxis.CategoryType = CategoryType.TimeScale;
            chart.CategoryAxis.MajorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MajorUnit = 2;
            
            workbook.Save("AxisPropertyMajorUnitScaleDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TimeUnit](../../timeunit/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


