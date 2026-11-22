---
title: "ChartPoint.GetBottomPointCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ChartPoint. تحصل على عدد النقاط السفلية بعد استدعاء طريقة Chart.Calculate"
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/getbottompointcount/
---
## ChartPoint.GetBottomPointCount method

يحصل على عدد النقاط السفلية بعد استدعاء طريقة Chart.Calculate().

```csharp
public int GetBottomPointCount()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetBottomPointCountDemo
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
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // احسب المخطط لضمان حساب جميع النقاط
            chart.Calculate();
            
            try
            {
                // احصل على النقطة الأولى في السلسلة الأولى.
                ChartPoint point = chart.NSeries[0].Points[0];
                
                // استدعِ طريقة GetBottomPointCount
                int bottomPointCount = point.GetBottomPointCount();
                
                // اعرض النتيجة
                Console.WriteLine($"Number of bottom points: {bottomPointCount}");
                
                // اعرض إحداثيات النقاط السفلية
                for (int i = 0; i < bottomPointCount; i++)
                {
                    float x = point.GetBottomPointXPx(i);
                    float y = point.GetBottomPointYPx(i);
                    Console.WriteLine($"Bottom point {i}: X={x}, Y={y}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBottomPointCount method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("MethodGetBottomPointCountDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


