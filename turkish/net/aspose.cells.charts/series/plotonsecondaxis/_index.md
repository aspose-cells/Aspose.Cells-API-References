---
title: "Series.PlotOnSecondAxis"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. Bu serinin ikinci değer ekseninde çizilip çizilmediğini gösterir"
type: docs
url: /tr/net/aspose.cells.charts/series/plotonsecondaxis/
---
## Series.PlotOnSecondAxis property

Bu serinin ikinci değer ekseninde çizilip çizilmediğini gösterir.

```csharp
public bool PlotOnSecondAxis { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyPlotOnSecondAxisDemo
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
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Grafiğe seri ekle
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // İlk seriyi ikincil eksende çizecek şekilde ayarlayın
            chart.NSeries[0].PlotOnSecondAxis = true;

            // Çalışma kitabını kaydedin
            workbook.Save("SeriesPropertyPlotOnSecondAxisDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


