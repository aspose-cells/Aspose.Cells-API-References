---
title: "Series.Bar3DShapeType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. 3D çubuk veya sütun grafiğinde kullanılan 3D şekil tipini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/series/bar3dshapetype/
---
## Series.Bar3DShapeType property

3-D çubuk veya sütun grafiğiyle kullanılan 3D şekil tipini alır veya ayarlar.

```csharp
public Bar3DShapeType Bar3DShapeType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBar3DShapeTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // 3D çubuk grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Çubuk şekil tipini Silindir olarak ayarla
            chart.NSeries[0].Bar3DShapeType = Bar3DShapeType.Cylinder;

            // Çalışma kitabını kaydedin
            workbook.Save("Bar3DShapeTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* enum [Bar3DShapeType](../../bar3dshapetype/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


