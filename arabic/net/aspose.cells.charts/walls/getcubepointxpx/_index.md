---
title: "Walls.GetCubePointXPx"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Walls. تحصل على إحداثي x لنقطة القمة لمكعب الجدران بعد استدعاء طريقة Chart.Calculate. عدد نقاط القمة لمكعب الجدران هو ثمانية"
type: docs
url: /ar/net/aspose.cells.charts/walls/getcubepointxpx/
---
## Walls.GetCubePointXPx method

يحصل على الإحداثي السيني لنقطة القمة لمكعب الجدران بعد استدعاء طريقة Chart.Calculate(). عدد نقاط القمة لمكعب الجدران هو ثمانية

```csharp
public float GetCubePointXPx(int index)
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class WallsMethodGetCubePointXPxWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);
            worksheet.Cells["B5"].PutValue(4000);

            // إنشاء مخطط ثلاثي الأبعاد
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // احسب المخطط لضمان توفر خصائص الجدار
            chart.Calculate();

            // احصل على كائن Walls
            Walls walls = chart.Walls;

            try
            {
                // احصل على عدد نقاط المكعب
                int pointCount = walls.GetCubePointCount();

                if (pointCount > 0)
                {
                    // استدعِ GetCubePointXPx مع الفهرس 0 (النقطة الأولى)
                    float xCoordinate = walls.GetCubePointXPx(0);
                    
                    Console.WriteLine($"X coordinate of first cube point in pixels: {xCoordinate}");
                    Console.WriteLine("Method executed successfully with parameter (Int32)");
                }
                else
                {
                    Console.WriteLine("No cube points available in the walls");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCubePointXPx method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("WallsMethodGetCubePointXPxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


