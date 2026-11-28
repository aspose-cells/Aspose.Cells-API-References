---
title: "Series.Overlap"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. Çubuk ve sütunların nasıl konumlandırıldığını belirtir. 100 ile 100 arasında bir değer olabilir. Yalnızca 2D çubuk ve 2D sütun grafiklerinde uygulanır"
type: docs
url: /tr/net/aspose.cells.charts/series/overlap/
---
## Series.Overlap property

Çubukların ve sütunların nasıl konumlandırılacağını belirtir. -100 ile 100 arasında bir değer olabilir. Yalnızca 2D çubuk ve 2D sütun grafiklerinde uygulanır.

```csharp
public short Overlap { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyOverlapDemo
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
            sheet.Cells["B1"].PutValue("Series1");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);
            sheet.Cells["C1"].PutValue("Series2");
            sheet.Cells["C2"].PutValue(15);
            sheet.Cells["C3"].PutValue(25);
            sheet.Cells["C4"].PutValue(35);

            // Kümelenmiş bir sütun grafiği ekleyin
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // İlk serinin çakışma özelliğini ayarlayın
            chart.NSeries[0].Overlap = -40;

            // Çalışma kitabını kaydedin
            workbook.Save("SeriesOverlapDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


