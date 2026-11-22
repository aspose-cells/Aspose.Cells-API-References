---
title: "ChartPoint.ShapeWidthPx"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. تحصل على العرض بوحدات البكسل بعد استدعاء طريقة Chart.Calculate"
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/shapewidthpx/
---
## ChartPoint.ShapeWidthPx property

يحصل على العرض بوحدات البكسل بعد استدعاء طريقة Chart.Calculate().

```csharp
public int ShapeWidthPx { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeWidthPxDemo
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

            // احسب المخطط لضمان توفر خصائص الشكل.
            chart.Calculate();

            // احصل على أول نقطة مخطط من السلسلة الأولى
            ChartPoint point = chart.NSeries[0].Points[0];

            // عرض العرض الحالي لشكل نقطة المخطط بوحدات البكسل
            Console.WriteLine("Current ShapeWidthPx value: " + point.ShapeWidthPx);

            // ملاحظة: ShapeWidthPx للقراءة فقط، لذا لا يمكن تعيينه مباشرة
            // لتغيير العرض، نحتاج إلى تعديل حجم المخطط أو خصائص أخرى
            // سيؤثر ذلك على عرض النقطة أثناء الاستدعاء التالي لـ Calculate()

            // غيّر عرض المخطط لتوضيح كيف يؤثر ذلك على ShapeWidthPx
            chart.ChartObject.Width = 1000;
            chart.Calculate();

            // عرض العرض الجديد بعد تغيير حجم المخطط
            Console.WriteLine("New ShapeWidthPx value after chart resize: " + point.ShapeWidthPx);

            // حفظ النتيجة
            workbook.Save("ChartPointPropertyShapeWidthPxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


