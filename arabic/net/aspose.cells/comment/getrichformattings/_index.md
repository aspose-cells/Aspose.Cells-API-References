---
title: "Comment.GetRichFormattings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Comment. تُرجع جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل نص التعليق"
type: docs
url: /ar/net/aspose.cells/comment/getrichformattings/
---
## Comment.GetRichFormattings method

يرجع جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل نص التعليق.

```csharp
public FontSetting[] GetRichFormattings()
```

### قيمة الإرجاع

جميع كائنات Characters

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentMethodGetRichFormattingsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تعليق إلى الخلية A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.HtmlNote = "<b>Bold</b>, <i>Italic</i>, <u>Underline</u>";

            // احصل على تنسيقات النص الغني
            FontSetting[] formattings = comment.GetRichFormattings();

            // عرض معلومات التنسيق
            Console.WriteLine("Rich Text Formattings:");
            foreach (FontSetting setting in formattings)
            {
                Console.WriteLine($"StartIndex: {setting.StartIndex}, Length: {setting.Length}");
                Console.WriteLine($"Bold: {setting.Font.IsBold}, Italic: {setting.Font.IsItalic}, Underline: {setting.Font.Underline}");
            }
        }
    }
}
```

### انظر أيضًا

* class [FontSetting](../../fontsetting/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


