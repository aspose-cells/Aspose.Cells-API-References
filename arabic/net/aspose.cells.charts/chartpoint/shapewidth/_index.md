---
title: "ChartPoint.ShapeWidth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. يحصل على العرض بوحدات 1/4000 من عرض المخطط بعد استدعاء طريقة Chart.Calculate"
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/shapewidth/
---
## ChartPoint.ShapeWidth property

يحصل على العرض بوحدات 1/4000 من عرض المخطط بعد استدعاء طريقة Chart.Calculate().

```csharp
public int ShapeWidth { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeWidthDemo
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
            
            // احسب المخطط لضمان توفر خصائص الشكل.
            chart.Calculate();
            
            // احصل على أول نقطة في المخطط في السلسلة الأولى
            ChartPoint point = chart.NSeries[0].Points[0];
            
            // اعرض القيمة الحالية لـ ShapeWidth (بوحدة 1/4000 من عرض المخطط)
            Console.WriteLine("Current ShapeWidth value: " + point.ShapeWidth);
            
            // اعرض العرض بوحدات البكسل
            Console.WriteLine("Shape width in pixels: " + point.ShapeWidthPx);
            
            // ملاحظة: ShapeWidth للقراءة فقط، لذا لا يمكننا تعيينه مباشرة
            // لتغيير العرض، سيتعين علينا تعديل حجم المخطط أو خصائص أخرى
            
            // حفظ النتيجة
            workbook.Save("ChartPointShapeWidthDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


