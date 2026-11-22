---
title: "Comment.TextVerticalAlignment"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Comment. تحصل وتعيّن نوع محاذاة النص العمودية للتعليق"
type: docs
url: /ar/net/aspose.cells/comment/textverticalalignment/
---
## Comment.TextVerticalAlignment property

يحصل ويضبط نوع محاذاة النص العمودية للتعليق.

```csharp
public TextAlignmentType TextVerticalAlignment { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyTextVerticalAlignmentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("B3");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment text";

            // عيّن المحاذاة العمودية إلى Fill
            comment.TextVerticalAlignment = TextAlignmentType.Fill;
            Console.WriteLine("Vertical Alignment: " + comment.TextVerticalAlignment);

            // غيّر المحاذاة العمودية إلى Center إذا كانت Fill
            if (comment.TextVerticalAlignment == TextAlignmentType.Fill)
            {
                comment.TextVerticalAlignment = TextAlignmentType.Center;
                Console.WriteLine("Changed Vertical Alignment to: " + comment.TextVerticalAlignment);
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


