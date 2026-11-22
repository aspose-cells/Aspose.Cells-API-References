---
title: "Comment.Author"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Comment. تحصل وتعيّن اسم مؤلف التعليق الأصلي"
type: docs
url: /ar/net/aspose.cells/comment/author/
---
## Comment.Author property

يحصل ويضبط اسم مؤلف التعليق الأصلي

```csharp
public string Author { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyAuthorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تعليق إلى الخلية A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // عيّن مؤلف التعليق والملاحظة
            comment.Author = "Carl.Yang";
            comment.Note = "This is a sample comment";

            // اعرض مؤلف التعليق
            Console.WriteLine("Comment Author: " + comment.Author);
        }
    }
}
```

### انظر أيضًا

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


