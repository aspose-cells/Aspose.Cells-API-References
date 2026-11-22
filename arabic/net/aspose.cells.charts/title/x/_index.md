---
title: "Title.X"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Title. تحصل أو تعين إحداثي X للزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/title/x/
---
## Title.X property

تحصل أو تعين إحداثي X للزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط.

```csharp
[Obsolete("Use Title.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int X { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهجورًا. يرجى استخدام خاصية Title.XRatioToChart بدلاً من ذلك. X = XRatioToChart * 4000; سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. تقدم Aspose اعتذارًا عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TitlePropertyXDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);

            // أضف مخططًا واضبط البيانات
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // اضبط خصائص عنوان المخطط مع موضع X
            chart.Title.Text = "Sample Chart";
            chart.Title.X = 200; // Demonstrating X property usage
            chart.Title.Y = 50;

            // احفظ المصنف
            workbook.Save("TitlePropertyXDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


