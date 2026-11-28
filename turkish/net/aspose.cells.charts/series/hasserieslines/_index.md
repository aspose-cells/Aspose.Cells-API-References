---
title: "Series.HasSeriesLines"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. Yığılmış sütun grafiği veya çubuk grafiğinde seri çizgileri varsa veya Pie of Pie grafiği ya da Bar of Pie grafiğinde iki bölüm arasında bağlayıcı çizgiler varsa doğru. Yalnızca yığılmış sütun grafikleri, çubuk grafikleri, Pie of Pie grafikleri veya Bar of Pie grafiklerinde uygulanır"
type: docs
url: /tr/net/aspose.cells.charts/series/hasserieslines/
---
## Series.HasSeriesLines property

Yığılmış sütun grafiği veya çubuk grafiğinde seri çizgileri varsa veya Pie of Pie grafiği ya da Bar of Pie grafiğinde iki bölüm arasında bağlayıcı çizgiler varsa doğrudur. Yalnızca yığılmış sütun grafikleri, çubuk grafikler, Pie of Pie grafikler veya Bar of Pie grafiklerinde uygulanır.

```csharp
public bool HasSeriesLines { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHasSeriesLinesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Q3");

            // Yığılmış bir sütun grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.ColumnStacked, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Seri verisi ekle
            chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "C1:C3";

            // İlk seriye erişin
            Series series = chart.NSeries[0];
            
            // HasSeriesLines özelliğini göster
            series.HasSeriesLines = true; // Enable series lines
            
            // Çalışma kitabını kaydedin
            workbook.Save("SeriesHasSeriesLinesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


