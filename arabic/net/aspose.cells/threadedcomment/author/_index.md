---
title: "ThreadedComment.Author"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreadedComment. تحصل على مؤلف التعليق"
type: docs
url: /ar/net/aspose.cells/threadedcomment/author/
---
## ThreadedComment.Author property

يحصل على مؤلف التعليق.

```csharp
public ThreadedCommentAuthor Author { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyAuthorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // الحصول على مؤلف التعليق المتسلسل الافتراضي من دفتر العمل
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                author.Name = "John Doe";
                author.UserId = "john.doe@example.com";

                // إضافة تعليق متسلسل إلى الخلية A1 (الصف 0، العمود 0)
                worksheet.Comments.AddThreadedComment(0, 0, "Sample comment", author);

                // الحصول على أول تعليق متسلسل
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];

                // عرض قيمة خاصية Author (عملية قراءة)
                Console.WriteLine("Author Name: " + comment.Author.Name);
                Console.WriteLine("Author UserId: " + comment.Author.UserId);
                Console.WriteLine("Author ProviderId: " + comment.Author.ProviderId);

                // إظهار تعيين خاصية Author (نظرًا لأنها قراءة/كتابة)
                ThreadedCommentAuthor newAuthor = workbook.Worksheets.ThreadedCommentAuthors[0];
                newAuthor.Name = "Jane Smith";
                newAuthor.UserId = "jane.smith@example.com";
                comment.Author = newAuthor;

                // عرض قيمة خاصية Author المحدثة
                Console.WriteLine("Updated Author Name: " + comment.Author.Name);
                Console.WriteLine("Updated Author UserId: " + comment.Author.UserId);

                // احفظ المصنف
                workbook.Save("ThreadedCommentAuthorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


