---
title: "ChartPoint.InnerArcStartPointYPx"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. تحصل على إحداثي y لنقطة البداية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate. ينطبق على مخطط الدونات"
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/innerarcstartpointypx/
---
## ChartPoint.InnerArcStartPointYPx property

يحصل على إحداثي y لنقطة البدء لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخطط الدونات.

```csharp
public float InnerArcStartPointYPx { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcStartPointYPxDemo
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
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احسب المخطط لضمان تعبئة الخصائص
            chart.Calculate();

            // احصل على أول نقطة في المخطط
            ChartPoint point = chart.NSeries[0].Points[0];

            // اعرض قيمة InnerArcStartPointYPx
            Console.WriteLine("InnerArcStartPointYPx: " + point.InnerArcStartPointYPx);

            // ملاحظة: InnerArcStartPointYPx للقراءة فقط، لذا لا يمكننا تعيينه مباشرة
            // لتغيير الموقع، نحتاج إلى تعديل حجم فتحة الدونات
            chart.NSeries[0].DoughnutHoleSize = 50; // Percentage of the chart size

            // أعد حساب المخطط لتحديث الخصائص
            chart.Calculate();

            // اعرض قيمة InnerArcStartPointYPx الجديدة بعد تعديل حجم الفتحة
            Console.WriteLine("New InnerArcStartPointYPx after changing hole size: " + point.InnerArcStartPointYPx);

            // احفظ المصنف
            workbook.Save("ChartPointPropertyInnerArcStartPointYPxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


