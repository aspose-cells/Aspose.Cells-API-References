---
title: "Series.IsAutoSplit"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. Eşik değerinin otomatik olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.charts/series/isautosplit/
---
## Series.IsAutoSplit property

Eşik değerinin otomatik olup olmadığını gösterir.

```csharp
public bool IsAutoSplit { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyIsAutoSplitDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["A5"].PutValue("Grape");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Bir pasta grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // İlk seriye erişin ve IsAutoSplit özelliğini gösterin
            Series series = chart.NSeries[0];
            bool isAutoSplit = series.IsAutoSplit; // Get the value instead of setting it
            series.SplitValue = 25; // Split at value 25

            Console.WriteLine($"IsAutoSplit value: {isAutoSplit}");

            // Çalışma kitabını kaydedin
            workbook.Save("SeriesPropertyIsAutoSplitDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


