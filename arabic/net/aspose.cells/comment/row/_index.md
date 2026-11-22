---
title: "Comment.Row"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Comment. تحصل على فهرس الصف للتعليق"
type: docs
url: /ar/net/aspose.cells/comment/row/
---
## Comment.Row property

يحصل على فهرس الصف للتعليق.

```csharp
public int Row { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تعليق إلى الخلية A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            comment1.Note = "This is a sample comment";

            // احصل على فهرس الصف للخلية التي تم التعليق عليها وعرضه
            int row = comment1.Row;
            Console.WriteLine("The comment is in row: " + row);

            // أضف تعليقًا آخر إلى الخلية B3
            commentIndex = worksheet.Comments.Add("B3");
            Comment comment2 = worksheet.Comments[commentIndex];
            comment2.Note = "Another comment";

            // اعرض فهرس الصف للتعليق الثاني
            Console.WriteLine("Second comment is in row: " + comment2.Row);
        }
    }
}
```

### انظر أيضًا

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


