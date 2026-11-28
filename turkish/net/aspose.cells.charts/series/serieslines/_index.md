---
title: "Series.SeriesLines"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. Yığılmış çubuk grafiği veya yığılmış sütun grafiği için seri çizgilerini temsil eden bir SeriesLines nesnesi döndürür. Yalnızca yığılmış çubuk ve yığılmış sütun grafiklerine uygulanır"
type: docs
url: /tr/net/aspose.cells.charts/series/serieslines/
---
## Series.SeriesLines property

Yığılmış çubuk grafiği veya yığılmış sütun grafiği için seri çizgilerini temsil eden bir SeriesLines nesnesi döndürür. Yalnızca yığılmış çubuk ve yığılmış sütun grafiklerine uygulanır.

```csharp
public Line SeriesLines { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertySeriesLinesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["A5"].PutValue(4);
            
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Grafik oluştur
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Seri ekle
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // Seri çizgilerini özelleştir
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.SeriesLines.Color = Color.Red;
            series.SeriesLines.Weight = Aspose.Cells.Drawing.WeightType.SingleLine;
            
            // Çalışma kitabını kaydedin
            workbook.Save("SeriesLinesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


