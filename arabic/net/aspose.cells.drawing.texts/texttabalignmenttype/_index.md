---
title: "التعداد TextTabAlignmentType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.Texts.TextTabAlignmentType. يمثل أنواع محاذاة علامات التبويب النصية."
type: docs
url: /ar/net/aspose.cells.drawing.texts/texttabalignmenttype/
---
## TextTabAlignmentType enumeration

يمثل أنواع محاذاة تبويب النص.

```csharp
public enum TextTabAlignmentType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Center | `0` | النص عند هذه النقطة المتوسطة محاذى إلى الوسط. |
| Decimal | `1` | عند هذه النقطة المتوسطة، يتم محاذاة الكسور العشرية. |
| Left | `2` | النص عند هذه النقطة المتوسطة محاذى إلى اليسار. |
| Right | `3` | النص عند هذه النقطة المتوسطة محاذى إلى اليمين. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassTextTabAlignmentTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء صندوق نص لتوضيح محاذاة الفواصل.
            int textBoxIndex = worksheet.TextBoxes.Add(0, 0, 400, 300);
            var textBox = worksheet.TextBoxes[textBoxIndex];
            var paragraph = textBox.TextBody.TextParagraphs[0];

            // إضافة نقاط تبويب بأنواع محاذاة مختلفة.
            paragraph.Stops.Add(TextTabAlignmentType.Left, 100);
            paragraph.Stops.Add(TextTabAlignmentType.Center, 200);
            paragraph.Stops.Add(TextTabAlignmentType.Right, 300);
            paragraph.Stops.Add(TextTabAlignmentType.Decimal, 400);

            // تعيين النص لتوضيح جميع أنواع المحاذاة.
            textBox.Text = "Left\tCenter\tRight\tDecimal\n" +
                           "Data\tData\tData\t12.34\n" +
                           "More\tMore\tMore\t56.78";

            // تطبيق التنسيق لجعل الفواصل مرئية.
            textBox.Font.Size = 12;
            textBox.TextBody.TextParagraphs[0].AlignmentType = TextAlignmentType.Left;

            // حفظ النتيجة
            workbook.Save("TextTabAlignmentTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


