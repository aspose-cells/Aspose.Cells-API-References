---
title: "ChartPoint.ShapeX"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. تحصل على إحداثي x للزاوية العلوية اليسرى بوحدات 1/4000 من عرض المخطط بعد استدعاء طريقة Chart.Calculate."
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/shapex/
---
## ChartPoint.ShapeX property

يحصل على إحداثي x للزاوية العلوية اليسرى بوحدات 1/4000 من عرض المخطط بعد استدعاء طريقة Chart.Calculate().

```csharp
public int ShapeX { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeXDemo
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

            // احسب المخطط للتأكد من تعبئة ShapeX.
            chart.Calculate();

            // احصل على النقطة الأولى في السلسلة الأولى.
            ChartPoint point = chart.NSeries[0].Points[0];

            // اعرض قيمة ShapeX (1/4000 من عرض المخطط).
            Console.WriteLine("ShapeX value (1/4000 units): " + point.ShapeX);
            Console.WriteLine("ShapeX value (pixels): " + point.ShapeXPx);

            // أظهر استخدام ShapeX لتحديد موضع العناصر بالنسبة لنقطة المخطط.
            // ملاحظة: بما أن ShapeX للقراءة فقط، لا يمكننا تعديلها مباشرة،
            // لكن يمكننا استخدامها لتحديد موضع عناصر أخرى.
            if (point.ShapeX > 0)
            {
                // أضف مربع نص محاذى مع موضع X لنقطة المخطط.
                Aspose.Cells.Drawing.TextBox textBox = worksheet.Shapes.AddTextBox(
                    point.ShapeXPx, 100, 100, 50, 100, 50);
                textBox.Text = "Point 1";
            }

            // حفظ النتيجة
            workbook.Save("ChartPointShapeXDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


