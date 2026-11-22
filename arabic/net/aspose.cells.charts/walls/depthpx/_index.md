---
title: "Walls.DepthPx"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Walls. تحصل على العمق من الأمام إلى الخلف بوحدات البكسل بعد استدعاء طريقة Chart.Calculate"
type: docs
url: /ar/net/aspose.cells.charts/walls/depthpx/
---
## Walls.DepthPx property

يحصل على العمق من الأمام إلى الخلف بوحدات البكسل بعد استدعاء طريقة Chart.Calculate().

```csharp
public int DepthPx { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyDepthPxDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إنشاء مخطط ثلاثي الأبعاد
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احصل على الجدران وعرض خاصية DepthPx
            Walls walls = chart.Walls;
            Console.WriteLine("Wall Depth in Pixels: " + walls.DepthPx);

            // احفظ دفتر العمل
            workbook.Save("WallsDepthPxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


