---
title: "Series.Shadow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. Seri bir gölgeye sahipse doğru"
type: docs
url: /tr/net/aspose.cells.charts/series/shadow/
---
## Series.Shadow property

Serinin bir gölgesi varsa doğru.

```csharp
public bool Shadow { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyShadowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Grafik oluştur
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // İlk seriye erişin ve gölgeyi etkinleştirin
            Series series = chart.NSeries[0];
            series.Shadow = true;

            // Doğrulamak için kaydedin ve yeniden yükleyin
            workbook.Save("output.xlsx");
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Series loadedSeries = loadedWorkbook.Worksheets[0].Charts[0].NSeries[0];
            Console.WriteLine("Shadow enabled: " + loadedSeries.Shadow);
        }
    }
}
```

### Ayrıca Bakınız

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


