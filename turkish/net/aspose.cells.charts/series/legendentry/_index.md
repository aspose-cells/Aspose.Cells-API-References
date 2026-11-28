---
title: "Series.LegendEntry"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. Bu seriye göre lejand girişini alır"
type: docs
url: /tr/net/aspose.cells.charts/series/legendentry/
---
## Series.LegendEntry property

Bu seriye göre lejand girişini alır.

```csharp
public LegendEntry LegendEntry { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyLegendEntryDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // İlk seriyi al
            Series series = chart.NSeries[0];

            // LegendEntry işlevselliğini göster
            Console.WriteLine("LegendEntry.IsDeleted before: " + series.LegendEntry.IsDeleted);
            series.LegendEntry.IsDeleted = true;
            Console.WriteLine("LegendEntry.IsDeleted after setting to true: " + series.LegendEntry.IsDeleted);
            series.LegendEntry.IsDeleted = false;
            Console.WriteLine("LegendEntry.IsDeleted after setting to false: " + series.LegendEntry.IsDeleted);

            // Çalışma kitabını kaydedin
            workbook.Save("SeriesPropertyLegendEntryDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [LegendEntry](../../legendentry/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


