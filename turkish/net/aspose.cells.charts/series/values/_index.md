---
title: "Series.Values"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. Bu grafik serisinin Y değerlerini temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/series/values/
---
## Series.Values property

Bu grafik serisinin Y değerlerini temsil eder.

```csharp
public string Values { get; set; }
```

### Açıklamalar

Bu özellik tarafından tanımlanan gerçek değerleri (bu serinin her noktasına karşılık gelen) almak için lütfen [`PointValues`](../pointvalues/) kullanın.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyValuesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["C1"].PutValue("Series2");
            
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            worksheet.Cells["C2"].PutValue(15);
            worksheet.Cells["C3"].PutValue(25);
            worksheet.Cells["C4"].PutValue(35);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Values özelliğini kullanarak seri ekleyin
            chart.NSeries.Add("=Sheet1!$B$2:$B$4", true);
            chart.NSeries.Add("=Sheet1!$C$2:$C$4", true);

            // Kategori verisini ayarlayın
            chart.NSeries.CategoryData = "=Sheet1!$A$2:$A$4";

            // Her seri için Values özelliğini gösterin
            Console.WriteLine("Series 1 Values: " + chart.NSeries[0].Values);
            Console.WriteLine("Series 2 Values: " + chart.NSeries[1].Values);

            // Çalışma kitabını kaydedin
            workbook.Save("SeriesPropertyValuesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


