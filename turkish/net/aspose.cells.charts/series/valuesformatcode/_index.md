---
title: "Series.ValuesFormatCode"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. Values NumberList'in format kodunu temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/series/valuesformatcode/
---
## Series.ValuesFormatCode property

Values NumberList'in format kodunu temsil eder.

```csharp
public string ValuesFormatCode { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyValuesFormatCodeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(0.25);
            worksheet.Cells["B3"].PutValue(0.5);
            worksheet.Cells["B4"].PutValue(0.75);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // İlk seri için değer format kodunu ayarla
            chart.NSeries[0].ValuesFormatCode = "0.00%";

            // Çalışma kitabını kaydedin
            workbook.Save("SeriesPropertyValuesFormatCodeDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


