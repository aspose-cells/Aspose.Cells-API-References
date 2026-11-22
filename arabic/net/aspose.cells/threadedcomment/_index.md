---
title: "الفئة ThreadedComment"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.ThreadedComment. تمثل التعليق المتسلسل"
type: docs
url: /ar/net/aspose.cells/threadedcomment/
---
## ThreadedComment class

يمثل التعليق المتسلسل.

```csharp
public class ThreadedComment
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Author](../../aspose.cells/threadedcomment/author/) { get; set; } | يحصل على مؤلف التعليق. |
| [Column](../../aspose.cells/threadedcomment/column/) { get; } | يحصل على فهرس العمود للتعليق. |
| [CreatedTime](../../aspose.cells/threadedcomment/createdtime/) { get; set; } | يحصل ويضبط وقت الإنشاء لهذا التعليق المتسلسل. |
| [Notes](../../aspose.cells/threadedcomment/notes/) { get; set; } | يحصل ويضبط نص التعليق. |
| [Row](../../aspose.cells/threadedcomment/row/) { get; } | يحصل على فهرس الصف للتعليق. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassThreadedCommentDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة مؤلفين إلى المصنف
            int author1Id = workbook.Worksheets.ThreadedCommentAuthors.Add("User1", "user1@example.com", "1");
            int author2Id = workbook.Worksheets.ThreadedCommentAuthors.Add("User2", "", "2");
            
            // الحصول على مراجع المؤلف
            ThreadedCommentAuthor author1 = workbook.Worksheets.ThreadedCommentAuthors[author1Id];
            ThreadedCommentAuthor author2 = workbook.Worksheets.ThreadedCommentAuthors[author2Id];
            
            // إضافة تعليق إلى الخلية A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // إضافة تعليق متسلسل إلى التعليق
            int threadedCommentIndex = comment.ThreadedComments.Add("This is a threaded comment", author1);
            ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
            
            // عيّن الخصائص الإضافية
            threadedComment.Notes = "Additional notes";
            
            // إضافة رد إلى التعليق المتسلسل
            int replyIndex = comment.ThreadedComments.Add("This is a reply", author2);
            ThreadedComment reply = comment.ThreadedComments[replyIndex];
            
            // احفظ المصنف
            workbook.Save("ThreadedCommentDemo.xlsx");
            
            Console.WriteLine("Threaded comment demo completed.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


