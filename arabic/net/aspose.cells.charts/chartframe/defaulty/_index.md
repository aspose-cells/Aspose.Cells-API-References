---
title: "ChartFrame.DefaultY"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartFrame. تمثل y للموضع الافتراضي بوحدات 1/4000 من مساحة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartframe/defaulty/
---
## ChartFrame.DefaultY property

تمثل y للموضع الافتراضي بوحدات 1/4000 من مساحة المخطط.

```csharp
[Obsolete("Use ChartFrame.DefaultYRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultY { get; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهملًا. يرجى استخدام خاصية ChartFrame.DefaultYRatioToChart بدلاً من ذلك. DefaultY = (int)(DefaultYRatioToChart * 4000); سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. تُعرب Aspose عن أسفها لأي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultYDemo
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
            
            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // الوصول إلى عنوان المخطط الذي يرث من ChartFrame
            chart.Title.Text = "Sample Chart";
            ChartFrame chartFrame = chart.Title;
            
            // عرض قيمة DefaultY الحالية (خاصية للقراءة فقط)
            Console.WriteLine("DefaultY value (1/4000 of chart area): " + chartFrame.DefaultY);
            Console.WriteLine("DefaultY ratio to chart area: " + chartFrame.DefaultYRatioToChart);
            
            // إظهار كيف يؤثر DefaultY على التحديد بالمقارنة مع الموضع الحالي
            Console.WriteLine("Current Y position (ratio): " + chartFrame.YRatioToChart);
            
            // إعادة تعيين الموضع إلى الافتراضي باستخدام SetPositionAuto()
            chartFrame.SetPositionAuto();
            Console.WriteLine("Y position after reset (ratio): " + chartFrame.YRatioToChart);
            
            // حفظ النتيجة
            workbook.Save("ChartFramePropertyDefaultYDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


