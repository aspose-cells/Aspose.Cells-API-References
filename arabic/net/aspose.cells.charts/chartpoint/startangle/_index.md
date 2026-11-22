---
title: "ChartPoint.StartAngle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. تحصل على الزاوية الابتدائية لقسم الفطيرة مقاسة بالدرجات باتجاه عقارب الساعة من المحور السيني بعد استدعاء طريقة Chart.Calculate. ينطبق على مخطط الفطيرة"
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/startangle/
---
## ChartPoint.StartAngle property

يحصل على الزاوية الابتدائية لقسم الفطيرة، مقاسة بالدرجات باتجاه عقارب الساعة من محور x بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخطط الفطيرة.

```csharp
public float StartAngle { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyStartAngleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // إضافة مخطط فطيرة
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احسب المخطط لضمان تعبئة الخصائص
            chart.Calculate();

            // احصل على أول نقطة في المخطط
            ChartPoint point = chart.NSeries[0].Points[0];

            // اعرض قيمة StartAngle
            Console.WriteLine("StartAngle of first pie slice: " + point.StartAngle);

            // ملاحظة: StartAngle للقراءة فقط، لذا لا يمكننا تعيينه مباشرة
            // لتغيير الزاوية الابتدائية، نحتاج إلى تدوير مخطط الفطيرة بالكامل
            chart.NSeries[0].FirstSliceAngle = 90; // Rotate pie chart by 90 degrees

            // أعد الحساب لتحديث الزوايا
            chart.Calculate();

            // اعرض قيمة StartAngle الجديدة بعد الدوران
            Console.WriteLine("StartAngle after rotation: " + point.StartAngle);

            // احفظ المصنف
            workbook.Save("ChartPointPropertyStartAngleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


