---
title: "ChartFrame.DefaultX"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartFrame. تمثل x للموقع الافتراضي بوحدات 1/4000 من مساحة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartframe/defaultx/
---
## ChartFrame.DefaultX property

تمثل x للموقع الافتراضي بوحدات 1/4000 من مساحة المخطط.

```csharp
[Obsolete("Use ChartFrame.DefaultXRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultX { get; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهملًا. يرجى استخدام خاصية ChartFrame.DefaultXRatioToChart بدلاً من ذلك. DefaultX = (int)(DefaultXRatioToChart * 4000); سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultXDemo
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
            
            // الوصول إلى عنوان المخطط الذي يرث من ChartFrame
            chart.Title.Text = "Sample Chart";
            
            // عرض الموضع X الافتراضي لعنوان المخطط
            Console.WriteLine("Default X position (1/4000 of chart area): " + chart.Title.DefaultX);
            Console.WriteLine("Default X position (ratio of chart area): " + chart.Title.DefaultXRatioToChart);
            
            // إظهار كيف يؤثر الموضع الافتراضي على المخطط
            Console.WriteLine("Is default position set? " + chart.Title.IsDefaultPosBeSet);
            
            // تغيير موضع العنوان باستخدام خصائص النسبة (نظرًا لأن DefaultX للقراءة فقط)
            chart.Title.XRatioToChart = 0.2;
            chart.Title.YRatioToChart = 0.05;
            
            // احفظ المصنف
            workbook.Save("ChartFrameDefaultXDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


