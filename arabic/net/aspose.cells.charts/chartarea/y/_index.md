---
title: "ChartArea.Y"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartArea. تحصل أو تحصل على الإزاحة العمودية من الصف العلوي الأيسر بوحدات 1/4000 من مساحة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartarea/y/
---
## ChartArea.Y property

تحصل أو تحصل على الإزاحة العمودية من الصف العلوي الأيسر، بوحدات 1/4000 من مساحة المخطط.

```csharp
[Obsolete("Use ChartArea.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Y { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو الآن مهمل. يرجى استخدام خاصية ChartArea.YRatioToChart بدلاً من ذلك. Y = YRatioToChart * 4000; سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // تكوين مساحة المخطط باستخدام خاصية Y
            ChartArea chartArea = chart.ChartArea;
            chartArea.Y = 20; // Setting Y position
            chartArea.Height = 250;

            workbook.Save("ChartAreaYExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


