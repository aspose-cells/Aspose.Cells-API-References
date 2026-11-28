---
title: "Series.FirstSliceAngle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. İlk piechart veya doughnutchart diliminin açısını, dikeyden saat yönünde derece cinsinden alır veya ayarlar. Yalnızca pie, 3D pie ve doughnut grafiklerinde 0 ile 360 arasında değerlerle uygulanır"
type: docs
url: /tr/net/aspose.cells.charts/series/firstsliceangle/
---
## Series.FirstSliceAngle property

İlk pasta grafiği veya halka grafiği diliminin açısını derece cinsinden alır veya ayarlar (dikeyden saat yönünde). Yalnızca pasta, 3D pasta ve halka grafiklerinde uygulanır ve değer 0 ile 360 arasındadır.

```csharp
public short FirstSliceAngle { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyFirstSliceAngleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Pasta grafiği için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Pasta grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // İlk seriyi al ve FirstSliceAngle'ı ayarla
            Series series = chart.NSeries[0];
            series.FirstSliceAngle = 45; // Rotate pie chart by 45 degrees

            workbook.Save("PieChartWithFirstSliceAngle.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


