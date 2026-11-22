---
title: "ChartFrame.TextFont"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartFrame. يحصل على كائن Font للعنصر ChartFrame المحدد"
type: docs
url: /ar/net/aspose.cells.charts/chartframe/textfont/
---
## ChartFrame.TextFont property

يحصل على كائن [`Font`](../font/) للعنصر ChartFrame المحدد.

```csharp
[Obsolete("Use ChartFrame.Font property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual Font TextFont { get; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن غير صالح. بدلاً من ذلك، يرجى استخدام خاصية ChartFrame.Font. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2012. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyTextFontDemo
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

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // ضبط عنوان المخطط وتكوين الخط
            chart.Title.Text = "Sample Chart";
            chart.Title.TextFont.Name = "Arial";
            chart.Title.TextFont.Size = 14;
            chart.Title.TextFont.IsBold = true;
            chart.Title.TextFont.Color = System.Drawing.Color.Blue;

            // احفظ المصنف
            workbook.Save("ChartTitleFontDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Font](../../../aspose.cells/font/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


