---
title: "Walls.Height"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Walls. تحصل على الارتفاع من الأعلى إلى الأسفل بوحدات 1/4000 من ارتفاع المخطط بعد استدعاء طريقة Chart.Calculate"
type: docs
url: /ar/net/aspose.cells.charts/walls/height/
---
## Walls.Height property

يحصل على الارتفاع من الأعلى إلى الأسفل بوحدات 1/4000 من ارتفاع المخطط بعد استدعاء طريقة Chart.Calculate().

```csharp
public int Height { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyHeightDemo
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

            // إضافة مخطط ثلاثي الأبعاد
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.Calculate();

            // الوصول إلى الجدران وعرض خاصية Height
            Walls walls = chart.Walls;
            Console.WriteLine("Wall Height: " + walls.Height);
            Console.WriteLine("Wall Height in Pixels: " + walls.HeightPx);

            // عدّل حجم منطقة المخطط بدلاً من خاصية Height المباشرة
            chart.ChartObject.Height = 400;
            chart.Calculate();
            Console.WriteLine("After resizing - Wall Height: " + walls.Height);
            Console.WriteLine("After resizing - Wall Height in Pixels: " + walls.HeightPx);

            workbook.Save("WallsHeightDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


