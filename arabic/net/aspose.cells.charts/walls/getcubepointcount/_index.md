---
title: "Walls.GetCubePointCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Walls. تحصل على عدد نقاط المكعب بعد استدعاء طريقة Chart.Calculate"
type: docs
url: /ar/net/aspose.cells.charts/walls/getcubepointcount/
---
## Walls.GetCubePointCount method

يحصل على عدد نقاط المكعب بعد استدعاء طريقة Chart.Calculate().

```csharp
public int GetCubePointCount()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class WallsMethodGetCubePointCountDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط ثلاثي الأبعاد
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احسب المخطط لضمان توفر خصائص الجدار
            chart.Calculate();

            try
            {
                // احصل على كائن Walls
                Walls walls = chart.Walls;
                
                // استدعِ طريقة GetCubePointCount
                int pointCount = walls.GetCubePointCount();
                
                // اعرض النتيجة
                Console.WriteLine($"Number of cube points in chart walls: {pointCount}");
                
                // احفظ المصنف
                workbook.Save("WallsMethodGetCubePointCountDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCubePointCount method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


