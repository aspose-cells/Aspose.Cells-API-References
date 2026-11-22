---
title: "ChartPoint.ShapeY"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. تحصل على إحداثي y للزاوية العلوية اليسرى بوحدات 1/4000 من ارتفاع المخطط بعد استدعاء طريقة Chart.Calculate."
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/shapey/
---
## ChartPoint.ShapeY property

يحصل على إحداثي y للزاوية العلوية اليسرى بوحدات 1/4000 من ارتفاع المخطط بعد استدعاء طريقة Chart.Calculate().

```csharp
public int ShapeY { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeYDemo
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

            // احسب المخطط للحصول على مواضع الشكل
            chart.Calculate();

            // احصل على النقطة الأولى في السلسلة الأولى.
            ChartPoint point = chart.NSeries[0].Points[0];

            // اعرض قيمة ShapeY الحالية (1/4000 من ارتفاع المخطط).
            Console.WriteLine("Current ShapeY value: " + point.ShapeY);

            // ملاحظة: ShapeY للقراءة فقط، لذلك لا يمكننا تعيينها مباشرة.
            // لتغيير الموضع، سنحتاج إلى تعديل البيانات الأساسية أو خصائص المخطط.

            // أظهر كيف يرتبط ShapeY بالموقع الفعلي.
            Console.WriteLine("ShapeY in pixels: " + point.ShapeYPx);
            Console.WriteLine("Chart height in pixels: " + (point.ShapeYPx * 4000 / point.ShapeY));

            // حفظ النتيجة
            workbook.Save("ChartPointPropertyShapeYDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


