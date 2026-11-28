---
title: "Series.SplitType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. İkinci pasta veya çubukta hangi veri noktalarının bulunacağını belirlemek için bir değer döndürür veya ayarlar (pasta içinde pasta veya çubuk içinde çubuk grafik için)."
type: docs
url: /tr/net/aspose.cells.charts/series/splittype/
---
## Series.SplitType property

Pie of pie veya bar of pie grafiğinde ikinci dilim veya çubukta hangi veri noktalarının bulunacağını belirleyen bir değeri döndürür veya ayarlar.

```csharp
public ChartSplitType SplitType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySplitTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Bir pasta grafiği ekle
            int chartIndex = sheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // İlk seri için bölme tipini ayarlayın
            chart.NSeries[0].SplitType = ChartSplitType.Position;

            // Çalışma kitabını kaydedin
            workbook.Save("SeriesPropertySplitTypeDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ChartSplitType](../../chartsplittype/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


