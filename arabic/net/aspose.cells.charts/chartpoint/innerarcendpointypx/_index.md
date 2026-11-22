---
title: "ChartPoint.InnerArcEndPointYPx"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. تحصل على إحداثي y لنقطة النهاية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate. ينطبق على مخطط الدونات"
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/innerarcendpointypx/
---
## ChartPoint.InnerArcEndPointYPx property

يحصل على إحداثي y للنقطة النهائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخطط الدونات.

```csharp
public float InnerArcEndPointYPx { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcEndPointYPxDemo
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
            worksheet.Cells["B2"].PutValue(40);
            worksheet.Cells["B3"].PutValue(35);
            worksheet.Cells["B4"].PutValue(25);

            // أضف مخطط Doughnut
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احسب المخطط للحصول على خصائص نقاط المخطط
            chart.Calculate();

            // احصل على أول نقطة مخطط من السلسلة الأولى
            ChartPoint point = chart.NSeries[0].Points[0];

            // اعرض قيمة InnerArcEndPointYPx الحالية
            Console.WriteLine("Current InnerArcEndPointYPx value: " + point.InnerArcEndPointYPx);

            // ملاحظة: InnerArcEndPointYPx للقراءة فقط، لذا لا يمكننا تعيينه مباشرة
            // لتغيير الموقع، نحتاج إلى تعديل حجم فتحة الدونات
            chart.NSeries[0].DoughnutHoleSize = 60; // Change hole size to affect inner arc position

            // أعد حساب المخطط لتحديث الخصائص
            chart.Calculate();

            // اعرض قيمة InnerArcEndPointYPx الجديدة بعد تعديل حجم الفتحة
            Console.WriteLine("New InnerArcEndPointYPx value after changing hole size: " + point.InnerArcEndPointYPx);

            // احفظ المصنف
            workbook.Save("ChartPointPropertyInnerArcEndPointYPxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


