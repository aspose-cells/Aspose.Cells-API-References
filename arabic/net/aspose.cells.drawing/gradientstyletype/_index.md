---
title: "تعداد GradientStyleType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.GradientStyleType تعداد. يمثل نمط تظليل التدرج"
type: docs
url: /ar/net/aspose.cells.drawing/gradientstyletype/
---
## GradientStyleType enumeration

يمثل نمط تظليل التدرج.

```csharp
public enum GradientStyleType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| DiagonalDown | `0` | نمط تظليل قطري للأسفل |
| DiagonalUp | `1` | نمط تظليل قطري للأعلى |
| FromCenter | `2` | نمط تظليل من المركز |
| FromCorner | `3` | نمط تظليل من الزاوية |
| Horizontal | `4` | نمط تظليل أفقي |
| Vertical | `5` | نمط تظليل عمودي |
| Unknown | `6` | نمط تظليل غير معروف. فقط لنمط التظليل (الذي لا ينتمي إلى أي عضو من GradientStyleType) في ملف القالب. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStyleTypeDemo
    {
        public static void GradientStyleTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
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

            // تعيين نطاق بيانات المخطط
            chart.SetChartDataRange("A1:B4", true);

            // الوصول إلى منطقة رسم المخطط
            PlotArea plotArea = chart.PlotArea;

            // الوصول إلى تنسيق التعبئة لمنطقة الرسم
            FillFormat fillFormat = plotArea.Area.FillFormat;

            // تعيين تعبئة تدرج ذات لونين بنمط DiagonalDown
            fillFormat.SetTwoColorGradient(Color.Blue, Color.White, GradientStyleType.DiagonalDown, 1);

            // إخراج نمط التدرج المستخدم
            Console.WriteLine("Gradient Style: " + fillFormat.GradientStyle);

            // احفظ المصنف
            workbook.Save("GradientStyleTypeExample.xlsx");
            workbook.Save("GradientStyleTypeExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


