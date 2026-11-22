---
title: "ChartFrame.DefaultWidth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartFrame. تمثل عرض الموضع الافتراضي بوحدات 1/4000 من مساحة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartframe/defaultwidth/
---
## ChartFrame.DefaultWidth property

تمثل عرض الموضع الافتراضي بوحدات 1/4000 من مساحة المخطط.

```csharp
[Obsolete("Use ChartFrame.DefaultWidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultWidth { get; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهجورًا. يرجى استخدام الخاصية ChartFrame.DefaultWidthRatioToChart بدلاً من ذلك. DefaultWidth = (int)(DefaultWidthRatioToChart * 4000); سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultWidthDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            
            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // الوصول إلى عنوان المخطط (الذي يرث من ChartFrame)
            Title title = chart.Title;
            
            // عرض العرض الافتراضي لإطار المخطط (العنوان في هذه الحالة)
            Console.WriteLine("DefaultWidth of chart title: " + title.DefaultWidth);
            
            // ملاحظة: DefaultWidth للقراءة فقط، لذا لا يمكننا تعيينه
            // يمكننا فقط قراءته لفهم الأبعاد الافتراضية
            
            // إظهار كيف تؤثر هذه الخاصية على المخطط
            Console.WriteLine("IsDefaultPosBeSet: " + title.IsDefaultPosBeSet);
            Console.WriteLine("DefaultWidthRatioToChart: " + title.DefaultWidthRatioToChart);
            
            // احفظ المصنف
            workbook.Save("ChartFrameDefaultWidthDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


