---
title: "تعداد TextOverflowType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Drawing.TextOverflowType. يمثل طريقة تدفق النص عمودياً أو أفقياً"
type: docs
url: /ar/net/aspose.cells.drawing/textoverflowtype/
---
## TextOverflowType enumeration

يمثل طريقة تجاوز النص عمودياً أو أفقياً.

```csharp
public enum TextOverflowType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Clip | `0` | انتبه إلى الحواجز العلوية والسفلية. لا تقدم أي إشارة إلى وجود نص غير مرئي. |
| Ellipsis | `1` | انتبه إلى الحواجز العلوية والسفلية. استخدم ثلاث نقاط للإشارة إلى وجود نص غير مرئي. فقط لتدفق عمودي. |
| Overflow | `2` | تجاوز النص ولا تنتبه إلى الحواجز العلوية والسفلية. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DrawingClassTextOverflowTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // إضافة مربع نص إلى المخطط
            TextBox textBox = chart.Shapes.AddTextBoxInChart(10, 10, 200, 50);

            // تعيين خصائص مربع النص
            textBox.TextBody.TextAlignment.AutoSize = false;
            textBox.Text = "This is a long text that will demonstrate text overflow handling";
            
            // تعيين نوع تدفق النص
            textBox.TextVerticalOverflow = TextOverflowType.Clip;

            // احفظ المصنف
            workbook.Save("TextOverflowTypeDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


