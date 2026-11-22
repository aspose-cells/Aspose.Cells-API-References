---
title: "ThreadedCommentAuthor.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreadedCommentAuthor. يحصل على ويضبط الاسم"
type: docs
url: /ar/net/aspose.cells/threadedcommentauthor/name/
---
## ThreadedCommentAuthor.Name property

يحصل على الاسم ويضبطه.

```csharp
public string Name { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentAuthorPropertyNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تعليق وتعليقات متسلسلة
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Initial comment";
            ThreadedCommentCollection threadedComments = comment.ThreadedComments;
            
            // إضافة تعليقات متسلسلة بمؤلفين مختلفين
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            int author1Index = authors.Add("User1", "user1@example.com", "ID1");
            int author2Index = authors.Add("User2", "user2@example.com", "ID2");

            // إضافة تعليقات متسلسلة
            threadedComments.Add("Reply from User1", authors[author1Index]);
            threadedComments.Add("Reply from User2", authors[author2Index]);

            // عرض استخدام خاصية Name
            Console.WriteLine("First author name: " + threadedComments[0].Author.Name);
            Console.WriteLine("Second author name: " + threadedComments[1].Author.Name);

            // تغيير مؤلف التعليق الثاني
            threadedComments[1].Author = authors[author1Index];
            Console.WriteLine("Updated second author name: " + threadedComments[1].Author.Name);

            // احفظ المصنف
            workbook.Save("ThreadedCommentAuthorsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ThreadedCommentAuthor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


