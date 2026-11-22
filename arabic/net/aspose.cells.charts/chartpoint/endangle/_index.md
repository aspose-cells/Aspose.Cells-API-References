---
title: "ChartPoint.EndAngle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. يحصل على الزاوية النهائية لقسم الفطيرة مقاسة بالدرجات مع اتجاه عقارب الساعة من المحور x بعد استدعاء طريقة Chart.Calculate. ينطبق على مخطط Pie."
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/endangle/
---
## ChartPoint.EndAngle property

يحصل على الزاوية النهائية لقسم الفطيرة، مقاسة بالدرجات باتجاه عقارب الساعة من محور x بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخطط الفطيرة.

```csharp
public float EndAngle { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyEndAngleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة لمخطط الفطيرة
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // إضافة مخطط فطيرة
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احسب المخطط لضمان تعبئة الخصائص
            chart.Calculate();

            // احصل على أول نقطة في المخطط (شريحة Apple)
            ChartPoint point = chart.NSeries[0].Points[0];

            // اعرض قيمة EndAngle الحالية
            Console.WriteLine("Current EndAngle value: " + point.EndAngle);

            // ملاحظة: EndAngle للقراءة فقط، لذا لا يمكننا تعيينه مباشرةً
            // بدلاً من ذلك، سنوضح كيف يرتبط بشريحة الفطيرة

            // انفجر النقطة لرؤية كيف يؤثر ذلك على الزوايا
            point.Explosion = 20;
            chart.Calculate(); // Recalculate to update angles

            // اعرض قيمة EndAngle الجديدة بعد الانفجار
            Console.WriteLine("EndAngle after explosion: " + point.EndAngle);

            // احفظ المصنف
            workbook.Save("ChartPointEndAngleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


