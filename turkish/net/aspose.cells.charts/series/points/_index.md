---
title: "Series.Points"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. Bir grafikteki serideki nokta koleksiyonunu alır"
type: docs
url: /tr/net/aspose.cells.charts/series/points/
---
## Series.Points property

Bir grafikteki serideki nokta koleksiyonunu alır.

```csharp
public ChartPointCollection Points { get; }
```

### Açıklamalar

Grafik Pie of Pie veya Bar of Pie olduğunda, son nokta ilk pasta çizimindeki diğer noktadır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyPointsDemo
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
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // İlk seriye ve noktalarına erişin
            Series series = chart.NSeries[0];
            foreach (ChartPoint point in series.Points)
            {
                // Her noktaya veri etiketleri ekleyin
                point.DataLabels.ShowValue = true;
                point.DataLabels.ShowCellRange = true;
            }

            // Çalışma kitabını kaydedin
            workbook.Save("SeriesPropertyPointsDemo_Output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPointCollection](../../chartpointcollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


