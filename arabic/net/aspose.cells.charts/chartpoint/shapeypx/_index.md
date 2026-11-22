---
title: "ChartPoint.ShapeYPx"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. تحصل على إحداثي y للزاوية العليا اليسرى بوحدات البكسل بعد استدعاء طريقة Chart.Calculate"
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/shapeypx/
---
## ChartPoint.ShapeYPx property

يحصل على إحداثي y للزاوية العلوية اليسرى بوحدات البكسل بعد استدعاء طريقة Chart.Calculate().

```csharp
public int ShapeYPx { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeYPxDemo
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

            // احصل على أول نقطة في السلسلة الأولى
            ChartPoint point = chart.NSeries[0].Points[0];

            // اعرض موضع Y الحالي بوحدات البكسل
            Console.WriteLine("Current ShapeYPx value: " + point.ShapeYPx);

            // ملاحظة: ShapeYPx للقراءة فقط، لذا لا يمكن تعيينه مباشرة
            // لتغيير الموضع، نحتاج إلى تعديل حجم/موضع المخطط أو البيانات

            // أظهر التأثير بتغيير موضع المخطط الذي سيؤثر على مواضع النقاط
            chart.Move(2, 3, 17, 11); // Move chart to row 2, column 3
            chart.Calculate(); // Recalculate to update positions

            // اعرض موضع Y الجديد بعد تحريك المخطط
            Console.WriteLine("New ShapeYPx value after chart movement: " + point.ShapeYPx);

            // حفظ النتيجة
            workbook.Save("ChartPointShapeYPxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


