---
title: "ChartPoint.InnerArcEndPointXPx"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. يحصل على إحداثي x للنقطة النهائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate. ينطبق على مخططات Doughnut"
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/innerarcendpointxpx/
---
## ChartPoint.InnerArcEndPointXPx property

يحصل على إحداثي x للنقطة النهائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخططات الدونات.

```csharp
public float InnerArcEndPointXPx { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcEndPointXPxDemo
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
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(3);
            worksheet.Cells["B4"].PutValue(2);

            // أضف مخطط Doughnut
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احسب المخطط للحصول على خصائص نقاط المخطط
            chart.Calculate();

            // احصل على أول نقطة مخطط من السلسلة الأولى
            ChartPoint point = chart.NSeries[0].Points[0];

            // اعرض القيمة الحالية لـ InnerArcEndPointXPx
            Console.WriteLine("Current InnerArcEndPointXPx value: " + point.InnerArcEndPointXPx);

            // ملاحظة: InnerArcEndPointXPx للقراءة فقط، لذا لا يمكننا تعيينه مباشرة
            // لتغيير موضع نقطة النهاية، نحتاج إلى تعديل حجم فتحة الدونات
            chart.NSeries[0].DoughnutHoleSize = 50; // Set hole size to 50%

            // أعد حساب المخطط لتحديث الخصائص
            chart.Calculate();

            // اعرض القيمة الجديدة لـ InnerArcEndPointXPx بعد تغيير حجم الفتحة
            Console.WriteLine("New InnerArcEndPointXPx value after changing doughnut hole size: " + point.InnerArcEndPointXPx);

            // احفظ المصنف
            workbook.Save("ChartPointPropertyInnerArcEndPointXPxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


