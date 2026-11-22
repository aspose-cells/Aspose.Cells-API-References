---
title: "ChartPoint.ShapeHeight"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. تحصل على الارتفاع بوحدات 1/4000 من ارتفاع المخطط بعد استدعاء طريقة Chart.Calculate."
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/shapeheight/
---
## ChartPoint.ShapeHeight property

يحصل على الارتفاع بوحدات 1/4000 من ارتفاع المخطط بعد استدعاء طريقة Chart.Calculate().

```csharp
public int ShapeHeight { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeHeightDemo
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
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احسب المخطط لضمان توفر خصائص الشكل.
            chart.Calculate();

            // احصل على النقطة الأولى في السلسلة الأولى.
            ChartPoint point = chart.NSeries[0].Points[0];

            // اعرض قيمة ShapeHeight الحالية (بوحدة 1/4000 من ارتفاع المخطط).
            Console.WriteLine("Current ShapeHeight value: " + point.ShapeHeight);

            // ملاحظة: ShapeHeight للقراءة فقط، لذلك لا يمكننا تعيينها مباشرة.
            // لتغيير الارتفاع، نحتاج إلى تعديل حجم المخطط أو خصائص أخرى.

            // أظهر التأثير عن طريق تغيير ارتفاع المخطط.
            Console.WriteLine("Original chart height: " + chart.ChartObject.Height);
            chart.ChartObject.Height = 400;
            chart.Calculate(); // Recalculate to update shape properties

            // اعرض قيمة ShapeHeight الجديدة بعد تغيير ارتفاع المخطط.
            Console.WriteLine("New ShapeHeight value after chart resize: " + point.ShapeHeight);

            // حفظ النتيجة
            workbook.Save("ChartPointPropertyShapeHeightDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


