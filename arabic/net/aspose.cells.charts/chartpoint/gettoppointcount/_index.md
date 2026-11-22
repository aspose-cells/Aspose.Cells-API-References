---
title: "ChartPoint.GetTopPointCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ChartPoint. تحصل على عدد النقاط العليا بعد استدعاء طريقة Chart.Calculate"
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/gettoppointcount/
---
## ChartPoint.GetTopPointCount method

يحصل على عدد النقاط العليا بعد استدعاء طريقة Chart.Calculate().

```csharp
public int GetTopPointCount()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetTopPointCountDemo
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

            // احسب المخطط للتأكد من ضبط جميع الخصائص
            chart.Calculate();

            try
            {
                // احصل على النقطة الأولى في السلسلة الأولى.
                ChartPoint point = chart.NSeries[0].Points[0];
                
                // استدعِ طريقة GetTopPointCount
                int topPointCount = point.GetTopPointCount();
                
                // اعرض النتيجة
                Console.WriteLine($"Number of top points: {topPointCount}");
                
                // عرض كيفية الحصول على إحداثيات النقطة العليا
                if (topPointCount > 0)
                {
                    for (int i = 0; i < topPointCount; i++)
                    {
                        float x = point.GetTopPointXPx(i);
                        float y = point.GetTopPointYPx(i);
                        Console.WriteLine($"Top point {i + 1} coordinates: ({x}, {y})");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTopPointCount method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("MethodGetTopPointCountDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


