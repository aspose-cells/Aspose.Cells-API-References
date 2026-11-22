---
title: "عدد TextOrientationType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.TextOrientationType عدد. يعدد أنواع توجيه النص"
type: docs
url: /ar/net/aspose.cells/textorientationtype/
---
## TextOrientationType enumeration

يسرد أنواع توجيه النص.

```csharp
public enum TextOrientationType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| ClockWise | `0` | يدور النص بزاوية 90 درجة مع اتجاه عقارب الساعة. |
| CounterClockWise | `1` | يدور النص بزاوية 90 درجة عكس اتجاه عقارب الساعة. |
| NoRotation | `2` | يمثل القيمة الافتراضية. |
| TopToBottom | `3` | يعرض النص من أعلى إلى أسفل الخلية. نص مكدس. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextOrientationTypeDemo
    {
        public static void TextOrientationTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Hello, Aspose!");
            worksheet.Cells["A2"].PutValue("This is a test comment.");

            // إضافة تعليق إلى الخلية A1
            int commentIndex = worksheet.Comments.Add(0, 0);
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a comment with text orientation.";

            // تعيين أنواع توجيه نص مختلفة للتعليق
            comment.TextOrientationType = TextOrientationType.ClockWise;
            Console.WriteLine("Text Orientation: ClockWise");

            // احفظ المصنف
            workbook.Save("TextOrientationTypeExample_ClockWise.xlsx");

            // تغيير توجيه النص إلى عكس اتجاه عقارب الساعة
            comment.TextOrientationType = TextOrientationType.CounterClockWise;
            Console.WriteLine("Text Orientation: CounterClockWise");

            // احفظ المصنف
            workbook.Save("TextOrientationTypeExample_CounterClockWise.xlsx");

            // تغيير توجيه النص إلى بدون تدوير
            comment.TextOrientationType = TextOrientationType.NoRotation;
            Console.WriteLine("Text Orientation: NoRotation");

            // احفظ المصنف
            workbook.Save("TextOrientationTypeExample_NoRotation.xlsx");

            // تغيير توجيه النص إلى من الأعلى إلى الأسفل
            comment.TextOrientationType = TextOrientationType.TopToBottom;
            Console.WriteLine("Text Orientation: TopToBottom");

            // احفظ المصنف
            workbook.Save("TextOrientationTypeExample_TopToBottom.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


