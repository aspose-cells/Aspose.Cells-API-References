---
title: "ChartFrame.DefaultHeight"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartFrame. تمثل ارتفاع الموضع الافتراضي بوحدات 1/4000 من مساحة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartframe/defaultheight/
---
## ChartFrame.DefaultHeight property

تمثل ارتفاع الموضع الافتراضي بوحدات 1/4000 من مساحة المخطط.

```csharp
[Obsolete("Use ChartFrame.DefaultHeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultHeight { get; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهجورًا. يرجى استخدام الخاصية ChartFrame.DefaultHeightRatioToChart بدلاً من ذلك. DefaultHeight = (int)(DefaultHeightRatioToChart * 4000); سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultHeightDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى عنوان المخطط (الذي هو ChartFrame)
            ChartFrame chartTitle = chart.Title;
            
            // عرض قيمة DefaultHeight الحالية (خاصية للقراءة فقط)
            Console.WriteLine("Current DefaultHeight value: " + chartTitle.DefaultHeight);

            // إظهار كيف يؤثر DefaultHeight على تخطيط المخطط
            Console.WriteLine("DefaultHeightRatioToChart: " + chartTitle.DefaultHeightRatioToChart);
            Console.WriteLine("Current HeightRatioToChart: " + chartTitle.HeightRatioToChart);

            // ضبط الارتفاع باستخدام الخاصية القابلة للكتابة
            chartTitle.HeightRatioToChart = chartTitle.DefaultHeightRatioToChart * 1.5;
            Console.WriteLine("New HeightRatioToChart: " + chartTitle.HeightRatioToChart);

            // حفظ النتيجة
            workbook.Save("ChartFrameDefaultHeightDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


