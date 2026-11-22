---
title: "ChartPoint.ShapeXPx"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. تحصل على إحداثي x للزاوية العليا اليسرى بوحدات البكسل بعد استدعاء طريقة Chart.Calculate"
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/shapexpx/
---
## ChartPoint.ShapeXPx property

يحصل على إحداثي x للزاوية العلوية اليسرى بوحدات البكسل بعد استدعاء طريقة Chart.Calculate().

```csharp
public int ShapeXPx { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeXPxDemo
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

            // احسب المخطط للحصول على مواضع الأشكال
            chart.Calculate();

            // احصل على أول نقطة مخطط من السلسلة الأولى
            ChartPoint point = chart.NSeries[0].Points[0];

            // اعرض موضع X الحالي بالبكسل
            Console.WriteLine("Current ShapeXPx value: " + point.ShapeXPx);

            // ملاحظة: ShapeXPx للقراءة فقط، لذا لا يمكننا تعيينه مباشرة
            // لتغيير الموضع، سنحتاج إلى تعديل حجم/موضع المخطط أو البيانات

            // أظهر كيف تتغير الخاصية عندما نقوم بتعديل المخطط
            Console.WriteLine("\nChanging chart position...");
            chart.ChartObject.Left = 3;
            chart.ChartObject.Top = 2;
            chart.Calculate(); // Recalculate to update positions

            Console.WriteLine("New ShapeXPx value after chart move: " + point.ShapeXPx);

            // حفظ النتيجة
            workbook.Save("ChartPointPropertyShapeXPxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


