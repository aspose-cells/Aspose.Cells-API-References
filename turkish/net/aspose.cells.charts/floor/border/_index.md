---
title: "Floor.Border"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Floor özelliği. Kenar Çizgisini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/floor/border/
---
## Floor.Border property

Kenarı alır veya ayarlar [`Line`](../../../aspose.cells.drawing/line/).

```csharp
public Line Border { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FloorPropertyBorderDemo
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

            // 3D sütun grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafiğin Floor'ını al
            Floor floor = chart.Floor;

            // Yeni bir kenar eklemek yerine mevcut kenarı değiştirerek kenar özelliklerini ayarlayın
            floor.Border.Color = Color.Red;
            floor.Border.Weight = WeightType.MediumLine;
            floor.Border.DashType = MsoLineDashStyle.DashDot;
            floor.Border.IsVisible = true;
            floor.Border.Transparency = 0.5;

            // Çalışma kitabını kaydedin
            workbook.Save("FloorBorderDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Line](../../../aspose.cells.drawing/line/)
* class [Floor](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


