---
title: "ChartPoint.ShapeHeightPx"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. تحصل على الارتفاع بوحدات البكسل بعد استدعاء طريقة Chart.Calculate"
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/shapeheightpx/
---
## ChartPoint.ShapeHeightPx property

يحصل على الارتفاع بوحدات البكسل بعد استدعاء طريقة Chart.Calculate().

```csharp
public int ShapeHeightPx { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeHeightPxDemo
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

            // احسب المخطط للحصول على أبعاد الشكل
            chart.Calculate();

            // احصل على أول نقطة مخطط من السلسلة الأولى
            ChartPoint chartPoint = chart.NSeries[0].Points[0];

            // اعرض الارتفاع الحالي لشكل نقطة المخطط بوحدات البكسل
            Console.WriteLine("Current ShapeHeightPx value: " + chartPoint.ShapeHeightPx);

            // ملاحظة: ShapeHeightPx للقراءة فقط، لذلك لا يمكننا تعيينه مباشرةً
            // لتغيير الارتفاع، سيتعين علينا تعديل حجم المخطط أو قيم البيانات
            // وإعادة حساب المخطط

            // غيّر قيمة البيانات التي ستؤثر على حجم نقطة المخطط
            worksheet.Cells["B2"].PutValue(50);
            chart.Calculate();

            // اعرض الارتفاع الجديد بعد تغيير البيانات
            Console.WriteLine("New ShapeHeightPx value after data change: " + chartPoint.ShapeHeightPx);

            // احفظ المصنف
            workbook.Save("ChartPointShapeHeightPxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


