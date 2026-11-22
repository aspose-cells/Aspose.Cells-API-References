---
title: "ChartPoint.InnerRadiusPx"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. تحصل على نصف القطر الداخلي لشريحة الدونات بوحدات البكسل بعد استدعاء طريقة Chart.Calculate. ينطبق على مخطط الدونات."
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/innerradiuspx/
---
## ChartPoint.InnerRadiusPx property

تحصل على نصف القطر الداخلي لشريحة الدونات بوحدات البكسل بعد استدعاء طريقة Chart.Calculate() . ينطبق على مخطط الدونات.

```csharp
[Obsolete("Use ChartPoint.DoughnutInnerRadius property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int InnerRadiusPx { get; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية ChartPoint.DoughnutInnerRadius. سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من يونيو 2024. تقدم Aspose باعتذار عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerRadiusPxDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("C1");
            worksheet.Cells["A3"].PutValue("C2");
            worksheet.Cells["A4"].PutValue("C3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(3);
            worksheet.Cells["B4"].PutValue(5);

            // أضف مخطط Doughnut
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احسب المخطط للحصول على خصائص نقاط المخطط.
            chart.Calculate();

            // احصل على أول نقطة مخطط من السلسلة الأولى
            ChartPoint point = chart.NSeries[0].Points[0];

            // اعرض قيمة نصف القطر الداخلي الحالية (خاصية للقراءة فقط).
            Console.WriteLine("Current InnerRadiusPx value: " + point.InnerRadiusPx);

            // ملاحظة: InnerRadiusPx للقراءة فقط، لذا لا يمكننا تعيينها مباشرة.
            // لتغيير نصف القطر الداخلي، نحتاج إلى تعديل حجم فتحة الدونات.
            chart.NSeries[0].DoughnutHoleSize = 50; // Percentage of the chart size

            // أعد حساب المخطط لتحديث الخصائص
            chart.Calculate();

            // اعرض قيمة نصف القطر الداخلي الجديدة بعد تعديل حجم فتحة الدونات.
            Console.WriteLine("New InnerRadiusPx value after changing DoughnutHoleSize: " + point.InnerRadiusPx);

            // حفظ النتيجة
            workbook.Save("ChartPointPropertyInnerRadiusPxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


