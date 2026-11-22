---
title: "ChartPoint.GetBottomPointYPx"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ChartPoint. تحصل على إحداثي y للنقطة السفلية للشكل بعد استدعاء طريقة Chart.Calculate. ينطبق على المخططات ثلاثية الأبعاد Column3D Bar3D Cone Cylinder Pyramid"
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/getbottompointypx/
---
## ChartPoint.GetBottomPointYPx method

يحصل على إحداثي y للنقطة السفلية للشكل بعد استدعاء طريقة Chart.Calculate(). ينطبق على المخططات ثلاثية الأبعاد: Column3D, Bar3D, Cone, Cylinder, Pyramid

```csharp
public float GetBottomPointYPx(int index)
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetBottomPointYPxDemo
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
            
            // إضافة سلسلة
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // احسب المخطط لضمان حساب جميع النقاط
            chart.Calculate();
            
            // احصل على أول نقطة في السلسلة الأولى
            ChartPoint point = chart.NSeries[0].Points[0];
            
            try
            {
                // احصل على عدد النقاط السفلية
                int bottomPointCount = point.GetBottomPointCount();
                
                if (bottomPointCount > 0)
                {
                    // استدعِ GetBottomPointYPx مع الفهرس 0
                    float yPx = point.GetBottomPointYPx(0);
                    
                    Console.WriteLine($"Bottom point Y position in pixels: {yPx}");
                    Console.WriteLine("Method executed successfully with parameter (Int32)");
                }
                else
                {
                    Console.WriteLine("No bottom points available for this chart point");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBottomPointYPx method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("MethodGetBottomPointYPxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


