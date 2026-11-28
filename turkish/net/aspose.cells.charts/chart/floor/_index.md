---
title: "Chart.Floor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart özelliği. 3D bir grafiğin duvarlarını temsil eden bir Floor nesnesi döndürür"
type: docs
url: /tr/net/aspose.cells.charts/chart/floor/
---
## Chart.Floor property

Bir `Floor` nesnesi döndürür; bu nesne 3-D bir grafiğin duvarlarını temsil eder.

```csharp
public Floor Floor { get; }
```

### Açıklamalar

Bu özellik 3-D pasta grafiklerine uygulanmaz.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyFloorDemo
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

            // 3D sütun grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Kat özelliklerine erişin ve değiştirin
            Floor floor = chart.Floor;
            floor.FillFormat.SetTwoColorGradient(System.Drawing.Color.LightBlue, System.Drawing.Color.DarkBlue, GradientStyleType.Horizontal, 2);
            floor.Border.Color = System.Drawing.Color.Black;

            // Çalışma kitabını kaydedin
            workbook.Save("ChartFloorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Floor](../../floor/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


