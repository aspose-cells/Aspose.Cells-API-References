---
title: "ChartPoint.GetBottomPointXPx"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ChartPoint. تحصل على إحداثي x للنقطة السفلية للشكل بعد استدعاء طريقة Chart.Calculate. ينطبق على المخططات ثلاثية الأبعاد Column3D Bar3D Cone Cylinder Pyramid"
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/getbottompointxpx/
---
## ChartPoint.GetBottomPointXPx method

يحصل على إحداثي x للنقطة السفلية للشكل بعد استدعاء طريقة Chart.Calculate(). ينطبق على المخططات ثلاثية الأبعاد: Column3D, Bar3D, Cone, Cylinder, Pyramid

```csharp
public float GetBottomPointXPx(int index)
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetBottomPointXPxWithInt32Demo
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

            // أضف مخطط عمودي
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احسب المخطط لضمان تعيين جميع خصائص الموضع
            chart.Calculate();

            try
            {
                // احصل على أول نقطة مخطط من السلسلة الأولى
                ChartPoint point = chart.NSeries[0].Points[0];

                // احصل على عدد النقاط السفلية
                int bottomPointCount = point.GetBottomPointCount();

                if (bottomPointCount > 0)
                {
                    // استدعِ GetBottomPointXPx مع الفهرس 0
                    float xPos = point.GetBottomPointXPx(0);
                    Console.WriteLine($"X position of bottom point (pixels): {xPos}");
                }
                else
                {
                    Console.WriteLine("No bottom points available for this chart point");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBottomPointXPx method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("ChartPointMethodGetBottomPointXPxWithInt32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


