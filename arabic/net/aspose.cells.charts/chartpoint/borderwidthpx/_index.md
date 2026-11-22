---
title: "ChartPoint.BorderWidthPx"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. تحصل على عرض الحدود بوحدات البكسل بعد استدعاء طريقة Chart.Calculate"
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/borderwidthpx/
---
## ChartPoint.BorderWidthPx property

يحصل على عرض الحدود بوحدات البكسل بعد استدعاء طريقة Chart.Calculate().

```csharp
public int BorderWidthPx { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ChartPointPropertyBorderWidthPxDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);
            worksheet.Cells["B4"].PutValue(1800);
            worksheet.Cells["B5"].PutValue(2100);

            // إضافة مخطط وتعيين نطاق البيانات الخاص به
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // احسب المخطط لضمان تعبئة الخصائص
            chart.Calculate();

            // احصل على أول نقطة في المخطط في السلسلة الأولى
            ChartPoint point = chart.NSeries[0].Points[0];

            // عرض عرض الحدود الحالي
            Console.WriteLine("Current BorderWidthPx value: " + point.BorderWidthPx);

            // ملاحظة: BorderWidthPx للقراءة فقط، لذا لا يمكننا تعيينه مباشرة
            // بدلاً من ذلك، يمكننا تعديل الحدود عبر الخاصية Border
            if (point.Border != null)
            {
                // غيّر عرض الحدود عن طريق تعيين الوزن باستخدام تعداد WeightType
                point.Border.Weight = WeightType.MediumLine; // Medium weight border
            }

            // أعد الحساب لتحديث قيمة BorderWidthPx
            chart.Calculate();

            // عرض عرض الحدود الجديد بالبكسل
            Console.WriteLine("New BorderWidthPx value after modification: " + point.BorderWidthPx);

            // احفظ المصنف
            workbook.Save("ChartPointPropertyBorderWidthPxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


