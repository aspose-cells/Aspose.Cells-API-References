---
title: "ChartPoint.DoughnutInnerRadius"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. يحصل على نصف القطر الداخلي لشريحة الدونات بوحدات البكسل بعد استدعاء طريقة Chart.Calculate. ينطبق على مخطط الدونات"
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/doughnutinnerradius/
---
## ChartPoint.DoughnutInnerRadius property

يحصل على نصف القطر الداخلي لشريحة الدونات بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخطط الدونات.

```csharp
public int DoughnutInnerRadius { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyDoughnutInnerRadiusDemo
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
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احسب المخطط للحصول على نقاط المخطط
            chart.Calculate();

            // احصل على أول نقطة مخطط من السلسلة الأولى
            ChartPoint point = chart.NSeries[0].Points[0];

            // اعرض القيمة الحالية لـ DoughnutInnerRadius
            Console.WriteLine("Current DoughnutInnerRadius value: " + point.DoughnutInnerRadius);

            // ملاحظة: DoughnutInnerRadius للقراءة فقط، لذا لا يمكننا تعيينه مباشرة
            // لتغيير نصف القطر الداخلي، نحتاج إلى تعديل خاصية HoleSize للمخطط
            chart.FirstSliceAngle = 30; // Adjust the first slice angle instead since HoleSize isn't available

            // أعد حساب المخطط لتحديث DoughnutInnerRadius
            chart.Calculate();

            // اعرض القيمة المحدثة لـ DoughnutInnerRadius
            Console.WriteLine("Updated DoughnutInnerRadius value: " + point.DoughnutInnerRadius);

            // احفظ المصنف
            workbook.Save("DoughnutInnerRadiusDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


