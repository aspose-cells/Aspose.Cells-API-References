---
title: "Walls.GetCubePointYPx"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Walls. تحصل على إحداثي y لنقطة القمة لمكعب الجدران بعد استدعاء طريقة Chart.Calculate. عدد نقاط القمة لمكعب الجدران هو ثمانية"
type: docs
url: /ar/net/aspose.cells.charts/walls/getcubepointypx/
---
## Walls.GetCubePointYPx method

يحصل على الإحداثي الصادي لنقطة القمة لمكعب الجدران بعد استدعاء طريقة Chart.Calculate(). عدد نقاط القمة لمكعب الجدران هو ثمانية.

```csharp
public float GetCubePointYPx(int index)
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class WallsMethodGetCubePointYPxDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط ثلاثي الأبعاد
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احسب المخطط لضمان تعبئة خصائص الجدار
            chart.Calculate();

            // احصل على كائن Walls
            Walls walls = chart.Walls;

            try
            {
                // احصل على عدد نقاط المكعب
                int pointCount = walls.GetCubePointCount();

                if (pointCount > 0)
                {
                    // استدعِ GetCubePointYPx مع الفهرس الأول (0)
                    float yPx = walls.GetCubePointYPx(0);
                    Console.WriteLine($"Y-coordinate of first cube point in pixels: {yPx}");
                }
                else
                {
                    Console.WriteLine("No cube points available in the walls.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCubePointYPx method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("WallsMethodGetCubePointYPxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


