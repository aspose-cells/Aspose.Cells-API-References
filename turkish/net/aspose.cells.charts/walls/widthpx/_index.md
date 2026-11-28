---
title: "Walls.WidthPx"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Walls özelliği. Chart.Calculate metodunu çağırdıktan sonra soldan sağa genişliği piksel biriminde alır"
type: docs
url: /tr/net/aspose.cells.charts/walls/widthpx/
---
## Walls.WidthPx property

Chart.Calculate() metodunu çağırdıktan sonra sol‑sağ genişliği piksel biriminde alır.

```csharp
public int WidthPx { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyWidthPxDemo
    {
        public static void Run()
        {
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

            // 3D grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.Calculate();

            // Duvarları alın ve WidthPx özelliğini gösterin
            Walls walls = chart.Walls;
            Console.WriteLine("Wall width in pixels: " + walls.WidthPx);

            // Çalışma kitabını kaydet
            workbook.Save("WallsWidthPxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


