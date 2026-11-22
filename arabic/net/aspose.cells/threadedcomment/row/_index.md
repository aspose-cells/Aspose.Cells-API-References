---
title: "ThreadedComment.Row"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreadedComment. تحصل على فهرس الصف للتعليق"
type: docs
url: /ar/net/aspose.cells/threadedcomment/row/
---
## ThreadedComment.Row property

يحصل على فهرس الصف للتعليق.

```csharp
public int Row { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // إنشاء مؤلف تعليق متسلسل
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                author.Name = "Test Author";
                author.UserId = "test@example.com";
                
                // إضافة تعليق متسلسل إلى الخلية B2 (الصف 1، العمود 1)
                worksheet.Comments.AddThreadedComment(1, 1, "Sample threaded comment", author);
                
                // الحصول على أول تعليق متسلسل
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];
                
                // عرض قيمة خاصية Row (للقراءة فقط)
                Console.WriteLine("Threaded comment row index: " + comment.Row);
                
                // تحقق من أن فهرس الصف يطابق المكان الذي وضعنا فيه التعليق
                if (comment.Row == 1)
                {
                    Console.WriteLine("Comment is correctly placed in row 1");
                }
                
                // احفظ المصنف
                workbook.Save("ThreadedCommentRowDemo.xlsx");
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

* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


