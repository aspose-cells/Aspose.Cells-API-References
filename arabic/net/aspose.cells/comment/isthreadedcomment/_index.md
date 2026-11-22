---
title: "Comment.IsThreadedComment"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Comment. تشير إلى ما إذا كان هذا التعليق تعليقًا متسلسلًا"
type: docs
url: /ar/net/aspose.cells/comment/isthreadedcomment/
---
## Comment.IsThreadedComment property

يشير إلى ما إذا كان هذا التعليق تعليقًا متسلسلًا.

```csharp
public bool IsThreadedComment { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyIsThreadedCommentDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف تعليقًا عاديًا
            Comment regularComment = worksheet.Comments[worksheet.Comments.Add("A1")];
            regularComment.Note = "This is a regular comment";
            regularComment.Author = "User1";

            // أضف تعليقًا متسلسلًا (بافتراض أن الـ API يدعم إضافة التعليقات المتسلسلة)
            Comment threadedComment = worksheet.Comments[worksheet.Comments.Add("B1")];
            threadedComment.Note = "This is a threaded comment";
            threadedComment.Author = "User2";

            // تحقق من أنواع التعليقات
            Console.WriteLine("Comment at A1 is threaded: " + regularComment.IsThreadedComment);
            Console.WriteLine("Comment at B1 is threaded: " + threadedComment.IsThreadedComment);

            // معالجة التعليقات بناءً على نوعها
            foreach (Comment comment in worksheet.Comments)
            {
                if (comment.IsThreadedComment)
                {
                    Console.WriteLine($"Threaded comment found at {CellsHelper.CellIndexToName(comment.Row, comment.Column)}");
                    Console.WriteLine($"Author: {comment.Author}, Note: {comment.Note}");
                }
                else
                {
                    Console.WriteLine($"Regular comment found at {CellsHelper.CellIndexToName(comment.Row, comment.Column)}");
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


