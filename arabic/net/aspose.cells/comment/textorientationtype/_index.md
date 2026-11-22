---
title: "Comment.TextOrientationType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Comment. تحصل وتضبط نوع توجيه النص للتعليق"
type: docs
url: /ar/net/aspose.cells/comment/textorientationtype/
---
## Comment.TextOrientationType property

يحصل ويضبط نوع توجيه النص للتعليق.

```csharp
public TextOrientationType TextOrientationType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyTextOrientationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تعليق إلى الخلية A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment text";

            // تعيين التوجيه الأولي إلى NoRotation
            comment.TextOrientationType = TextOrientationType.NoRotation;
            Console.WriteLine("Initial orientation: " + comment.TextOrientationType);

            // غيّر الاتجاه إلى TopToBottom إذا كان حاليًا NoRotation
            if (comment.TextOrientationType == TextOrientationType.NoRotation)
            {
                comment.TextOrientationType = TextOrientationType.TopToBottom;
                Console.WriteLine("Changed orientation to: " + comment.TextOrientationType);
            }

            // احفظ المصنف
            workbook.Save("CommentOrientationDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TextOrientationType](../../textorientationtype/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


