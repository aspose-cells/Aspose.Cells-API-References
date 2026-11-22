---
title: "ThreadedCommentCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreadedCommentCollection. تحصل على التعليق المتسلسل حسب الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells/threadedcommentcollection/item/
---
## ThreadedCommentCollection indexer

يحصل على التعليق المتسلسل حسب الفهرس المحدد.

```csharp
public ThreadedComment this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تعليق
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "Initial comment";

            // إضافة تعليقات متسلسلة
            ThreadedCommentCollection threadedComments = comment.ThreadedComments;
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            
            // إضافة مؤلفين
            int author1Index = authors.Add("User1", "user1@example.com", "ID1");
            int author2Index = authors.Add("User2", "user2@example.com", "ID2");

            // إضافة تعليقات متسلسلة
            threadedComments.Add("Reply 1", authors[author1Index]);
            threadedComments.Add("Reply 2", authors[author2Index]);

            // عرض استخدام خاصية Item
            ThreadedComment firstComment = threadedComments[0];
            ThreadedComment secondComment = threadedComments[1];

            Console.WriteLine("First comment author: " + firstComment.Author.Name);
            Console.WriteLine("Second comment author: " + secondComment.Author.Name);

            // تعديل مؤلف التعليق الثاني
            secondComment.Author = authors[author1Index];
            Console.WriteLine("Updated second comment author: " + secondComment.Author.Name);

            // احفظ المصنف
            workbook.Save("ThreadedCommentsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ThreadedComment](../../threadedcomment/)
* class [ThreadedCommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


