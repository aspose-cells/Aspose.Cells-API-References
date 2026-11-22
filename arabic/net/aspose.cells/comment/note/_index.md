---
title: "Comment.Note"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Comment. تمثل محتوى التعليق"
type: docs
url: /ar/net/aspose.cells/comment/note/
---
## Comment.Note property

يمثل محتوى التعليق.

```csharp
public string Note { get; set; }
```

### ملاحظات

إذا كان هذا تعليقًا متسلسلًا، لا يمكن تغيير الملاحظة، وإلا لن يتمكن MS Excel من معالجته كتعليق متسلسل.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyNoteDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تعليق إلى الخلية A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            
            // تعيين الملاحظة للتعليق
            comment1.Note = "First note.";
            
            // تحقق من تعيين الملاحظة
            Console.WriteLine("Comment note: " + comment1.Note);
        }
    }
}
```

### انظر أيضًا

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


