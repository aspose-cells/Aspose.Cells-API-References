---
title: "التعداد TextFontAlignType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.Texts.TextFontAlignType. تمثّل الأنواع المختلفة لمحاذاة الخط"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textfontaligntype/
---
## TextFontAlignType enumeration

يمثل الأنواع المختلفة لمحاذاة الخط.

```csharp
public enum TextFontAlignType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Automatic | `0` | عندما يكون تدفق النص أفقيًا أو عموديًا بسيطًا يكون مثل fontBaseline، ولكن بالنسبة لأوضاع عمودية أخرى يكون مثل fontCenter. |
| Bottom | `1` | الأحرف مثبتة في أسفل السطر الواحد تمامًا. |
| Baseline | `2` | الأحرف مثبتة على الخط الأساسي السفلي لسطر واحد. |
| Center | `3` | الأحرف مثبتة بين الخطين الأساسيين لسطر واحد. |
| Top | `4` | الأحرف مثبتة على الخط الأساسي العلوي لسطر واحد. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassTextFontAlignTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء صناديق نصية بمحاذاة خطوط مختلفة
            var textBoxAuto = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            textBoxAuto.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Automatic;
            textBoxAuto.Text = "Automatic Alignment";

            var textBoxBottom = worksheet.Shapes.AddTextBox(0, 200, 100, 100, 200, 200);
            textBoxBottom.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Bottom;
            textBoxBottom.Text = "Bottom Alignment";

            var textBoxBaseline = worksheet.Shapes.AddTextBox(0, 400, 100, 100, 200, 200);
            textBoxBaseline.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Baseline;
            textBoxBaseline.Text = "Baseline Alignment";

            var textBoxCenter = worksheet.Shapes.AddTextBox(200, 0, 100, 100, 200, 200);
            textBoxCenter.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Center;
            textBoxCenter.Text = "Center Alignment";

            var textBoxTop = worksheet.Shapes.AddTextBox(200, 200, 100, 100, 200, 200);
            textBoxTop.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Top;
            textBoxTop.Text = "Top Alignment";

            // عرض جميع قيم التعداد في وحدة التحكم
            Console.WriteLine("TextFontAlignType values:");
            Console.WriteLine($"Automatic: {TextFontAlignType.Automatic}");
            Console.WriteLine($"Bottom: {TextFontAlignType.Bottom}");
            Console.WriteLine($"Baseline: {TextFontAlignType.Baseline}");
            Console.WriteLine($"Center: {TextFontAlignType.Center}");
            Console.WriteLine($"Top: {TextFontAlignType.Top}");

            // احفظ المصنف
            workbook.Save("TextFontAlignTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


