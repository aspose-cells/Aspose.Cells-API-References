---
title: "CommentCollection.GetThreadedComments"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CommentCollection. تحصل على التعليقات المتسلسلة حسب فهرس الصف والعمود"
type: docs
url: /ar/net/aspose.cells/commentcollection/getthreadedcomments/
---
## GetThreadedComments(int, int) {#getthreadedcomments}

يحصل على التعليقات المتسلسلة حسب فهرس الصف والعمود.

```csharp
public ThreadedCommentCollection GetThreadedComments(int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |
| عمود | Int32 | فهرس العمود. |

### أمثلة

```csharp

[C#]
ThreadedCommentCollection threadedComments1 = comments.GetThreadedComments(1, 1);
for (int i = 0; i < threadedComments1.Count; ++i)
{
    ThreadedComment tc = threadedComments1[i];
    string note = tc.Notes;
}
```

### انظر أيضًا

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetThreadedComments(string) {#getthreadedcomments_1}

يحصل على التعليقات المتسلسلة حسب اسم الخلية.

```csharp
public ThreadedCommentCollection GetThreadedComments(string cellName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | String | اسم الخلية. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodGetThreadedCommentsWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف مؤلف تعليق متسلسل واحصل على المؤلف حسب الفهرس
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD", "1");
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

            // أضف تعليقًا متسلسلًا إلى الخلية B2
            worksheet.Comments.AddThreadedComment("B2", "Initial comment", author);

            // احصل على جميع التعليقات المتسلسلة للخلية B2
            ThreadedCommentCollection threadedComments = worksheet.Comments.GetThreadedComments("B2");

            // اعرض التعليقات المتسلسلة
            foreach (ThreadedComment comment in threadedComments)
            {
                Console.WriteLine($"Comment by {comment.Author.Name}: {comment.Notes}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


