---
title: "ChartFrame.Y"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartFrame. تحصل أو تعين إحداثي y للزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartframe/y/
---
## ChartFrame.Y property

تحصل أو تعين إحداثي y للزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط.

```csharp
[Obsolete("Use ChartFrame.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Y { get; set; }
```

### ملاحظات

كيف يتم تحويل الوحدات من 1/4000 إلى بكسل؟ Y في البكسل = Y * Chart.ChartObject.Height / 4000d;

ملاحظة: هذا العضو أصبح الآن مهجورًا. يرجى استخدام الخاصية ChartFrame.YRatioToChart بدلاً من ذلك. Y = YRatioToChart * 4000. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyYDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["A2"].PutValue("A");
            cells["A3"].PutValue("B");
            cells["A4"].PutValue("C");
            cells["B1"].PutValue("Value");
            cells["B2"].PutValue(10);
            cells["B3"].PutValue(20);
            cells["B4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // الوصول إلى عنوان المخطط وتعيين موضع Y
            chart.Title.Text = "Sample Chart";
            chart.Title.Y = 1000; // Demonstrate Y property usage

            // احفظ المصنف
            workbook.Save("ChartFramePropertyYDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


