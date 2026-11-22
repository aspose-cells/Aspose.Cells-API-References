---
title: "CommentShape.Comment"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CommentShape. تحصل على كائن التعليق"
type: docs
url: /ar/net/aspose.cells.drawing/commentshape/comment/
---
## CommentShape.Comment property

يحصل على كائن التعليق.

```csharp
public Comment Comment { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CommentShapePropertyCommentDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تعليق إلى الخلية A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment";
            
            // احصل على شكل التعليق وبيّن خاصية Comment
            CommentShape commentShape = worksheet.Comments[commentIndex].CommentShape;
            Comment retrievedComment = commentShape.Comment;
            
            // اعرض نص التعليق
            Console.WriteLine("Comment Text: " + retrievedComment.Note);
        }
    }
}
```

### انظر أيضًا

* class [Comment](../../../aspose.cells/comment/)
* class [CommentShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


