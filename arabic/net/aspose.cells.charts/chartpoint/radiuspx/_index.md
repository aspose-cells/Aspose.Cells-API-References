---
title: "ChartPoint.RadiusPx"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. تحصل على نصف قطر الفطيرة الفقاعية أو الدونات بوحدات البكسل بعد استدعاء طريقة Chart.Calculate"
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/radiuspx/
---
## ChartPoint.RadiusPx property

يحصل على نصف قطر الفقاعة أو الفطيرة أو الدونات بوحدات البكسل بعد استدعاء طريقة Chart.Calculate().

```csharp
public int RadiusPx { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyRadiusPxDemo
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
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احسب المخطط لضمان تعبئة الخصائص
            chart.Calculate();

            // احصل على أول نقطة في المخطط
            ChartPoint point = chart.NSeries[0].Points[0];

            // اعرض قيمة نصف القطر الحالية
            Console.WriteLine("Current RadiusPx value: " + point.RadiusPx);

            // ملاحظة: RadiusPx للقراءة فقط، لذا لا يمكننا تعيينه مباشرة
            // لتغيير نصف القطر، نحتاج إلى تعديل حجم المخطط أو خصائص أخرى
            // التي تؤثر على حجم النقطة بشكل غير مباشر

            // مثال على كيفية تأثير تغيير حجم المخطط على نصف القطر
            Console.WriteLine("\nChanging chart size to demonstrate radius change...");
            chart.ChartObject.Width = 800;
            chart.ChartObject.Height = 600;
            chart.Calculate();

            // اعرض قيمة نصف القطر الجديدة بعد تغيير حجم المخطط
            Console.WriteLine("New RadiusPx value after chart resize: " + point.RadiusPx);

            // حفظ النتيجة
            workbook.Save("ChartPointPropertyRadiusPxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


