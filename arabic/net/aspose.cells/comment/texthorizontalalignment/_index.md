---
title: "Comment.TextHorizontalAlignment"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Comment. تحصل وتعيّن نوع محاذاة النص الأفقية للتعليق"
type: docs
url: /ar/net/aspose.cells/comment/texthorizontalalignment/
---
## Comment.TextHorizontalAlignment property

يحصل ويضبط نوع محاذاة النص الأفقية للتعليق.

```csharp
public TextAlignmentType TextHorizontalAlignment { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyTextHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تعليق إلى الخلية A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment text";

            // عيّن المحاذاة الأفقية الأولية إلى Fill
            comment.TextHorizontalAlignment = TextAlignmentType.Fill;
            Console.WriteLine("Initial alignment: " + comment.TextHorizontalAlignment);

            // غيّر المحاذاة إلى Center إذا كانت Fill
            if (comment.TextHorizontalAlignment == TextAlignmentType.Fill)
            {
                comment.TextHorizontalAlignment = TextAlignmentType.Center;
                Console.WriteLine("Updated alignment: " + comment.TextHorizontalAlignment);
            }
        }
    }
}
```

### انظر أيضًا

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


