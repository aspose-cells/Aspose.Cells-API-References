---
title: "ChartPoint.ArcStartPointYPx"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. يحصل على إحداثي y للنقطة البداية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate. ينطبق على مخطط Pie و Doughnut."
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/arcstartpointypx/
---
## ChartPoint.ArcStartPointYPx property

يحصل على إحداثي y للنقطة الابتدائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخطط الفطيرة والدونات.

```csharp
public float ArcStartPointYPx { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcStartPointYPxDemo
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

            // إضافة مخطط فطيرة
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احسب المخطط للحصول على مواضع الأشكال.
            chart.Calculate();

            // احصل على أول نقطة في المخطط
            ChartPoint point = chart.NSeries[0].Points[0];

            // اعرض القيمة الحالية لـ ArcStartPointYPx
            Console.WriteLine("Current ArcStartPointYPx value: " + point.ArcStartPointYPx);

            // ملاحظة: ArcStartPointYPx للقراءة فقط، لذلك لا يمكننا تعيينه مباشرةً
            // بدلاً من ذلك، سنوضح كيف يؤثر تغيير الخصائص الأخرى على ArcStartPointYPx

            // غيّر قيمة الانفجار لتعديل موضع شريحة الفطيرة
            point.Explosion = 20;

            // أعد حساب المخطط لتحديث المواقع
            chart.Calculate();

            // اعرض القيمة الجديدة لـ ArcStartPointYPx بعد تغيير الانفجار
            Console.WriteLine("New ArcStartPointYPx after explosion change: " + point.ArcStartPointYPx);

            // احفظ المصنف
            workbook.Save("ChartPointPropertyArcStartPointYPxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


