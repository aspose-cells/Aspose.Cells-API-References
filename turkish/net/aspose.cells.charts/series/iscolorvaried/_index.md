---
title: "Series.IsColorVaried"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. Noktaların renginin değişken olup olmadığını temsil eder. Grafik yalnızca bir seri içermeli veya bu grafik bir pasta grafiği olmalıdır"
type: docs
url: /tr/net/aspose.cells.charts/series/iscolorvaried/
---
## Series.IsColorVaried property

Nokta renklerinin değişken olup olmadığını temsil eder. Grafik yalnızca bir seri içermeli veya bu grafik bir pasta grafiği olmalıdır.

```csharp
public bool IsColorVaried { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyIsColorVariedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // İlk seri için IsColorVaried özelliğini ayarla
            chart.NSeries[0].IsColorVaried = true;

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");

            // Özelliği doğrula
            Console.WriteLine("IsColorVaried: " + chart.NSeries[0].IsColorVaried);
        }
    }
}
```

### Ayrıca Bakınız

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


