---
title: "Comment.Column"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Comment. تحصل على فهرس العمود للتعليق"
type: docs
url: /ar/net/aspose.cells/comment/column/
---
## Comment.Column property

يحصل على فهرس العمود للتعليق.

```csharp
public int Column { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف تعليقًا إلى الخلية B5 (فهرس العمود 1)
            int commentRow = 4;
            int commentColumn = 1;
            Comment comment = worksheet.Comments[worksheet.Comments.Add(commentRow, commentColumn)];

            // ضبط نص التعليق
            comment.Note = "This is a sample comment";

            // إظهار استخدام خاصية Column
            Console.WriteLine("Comment is in column: " + comment.Column);

            // تحقق من أن فهرس العمود يتطابق مع المكان الذي وضعناه فيه
            if (comment.Column == commentColumn)
            {
                Console.WriteLine("Column property correctly returns the comment's column index");
            }
        }
    }
}
```

### انظر أيضًا

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


