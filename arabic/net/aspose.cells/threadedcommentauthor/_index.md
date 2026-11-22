---
title: "الفئة ThreadedCommentAuthor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.ThreadedCommentAuthor. تمثل الشخص الذي ينشئ التعليقات المتسلسلة"
type: docs
url: /ar/net/aspose.cells/threadedcommentauthor/
---
## ThreadedCommentAuthor class

يمثل الشخص الذي ينشئ التعليقات المتسلسلة.

```csharp
public class ThreadedCommentAuthor
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Name](../../aspose.cells/threadedcommentauthor/name/) { get; set; } | يحصل على الاسم ويضبطه. |
| [ProviderId](../../aspose.cells/threadedcommentauthor/providerid/) { get; set; } | يحصل على معرف الموفر. |
| [UserId](../../aspose.cells/threadedcommentauthor/userid/) { get; set; } | يحصل على معرف المستخدم ويضبطه. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassThreadedCommentAuthorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تعليق
            int commentIndex = worksheet.Comments.Add("C1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Initial comment";
            
            // إضافة مؤلفي التعليقات المتسلسلة
            int authorIndex1 = workbook.Worksheets.ThreadedCommentAuthors.Add("Author1", "user1", "");
            ThreadedCommentAuthor author1 = workbook.Worksheets.ThreadedCommentAuthors[authorIndex1];
            
            // إضافة تعليق متسلسل
            int threadedCommentIndex = comment.ThreadedComments.Add("Threaded comment text", author1);
            ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
            
            // الوصول إلى المؤلف وتعديله
            Console.WriteLine("Original author: " + threadedComment.Author.Name);
            threadedComment.Author.Name = "ModifiedAuthor";
            Console.WriteLine("Modified author: " + threadedComment.Author.Name);

            // إنشاء مؤلف جديد وتعيينه
            int authorIndex2 = workbook.Worksheets.ThreadedCommentAuthors.Add("Author2", "user2", "");
            ThreadedCommentAuthor author2 = workbook.Worksheets.ThreadedCommentAuthors[authorIndex2];
            threadedComment.Author = author2;
            Console.WriteLine("New author: " + threadedComment.Author.Name);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


