---
title: "ThreadedComment.Column"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreadedComment. تحصل على فهرس العمود للتعليق"
type: docs
url: /ar/net/aspose.cells/threadedcomment/column/
---
## ThreadedComment.Column property

يحصل على فهرس العمود للتعليق.

```csharp
public int Column { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // أنشئ مؤلف تعليق متسلسل أولاً
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                
                // إضافة تعليق متسلسل إلى الخلية A1 (الصف 0، العمود 0)
                int commentRow = 0;
                int commentColumn = 0;
                worksheet.Comments.AddThreadedComment(commentRow, commentColumn, "Sample comment text", author);
                
                // الحصول على أول تعليق متسلسل
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];
                
                // اعرض قيمة خاصية Column (للقراءة فقط)
                Console.WriteLine("Threaded comment column index: " + comment.Column);
                
                // تحقق من أن فهرس العمود يطابق المكان الذي وضعنا فيه التعليق
                if (comment.Column == commentColumn)
                {
                    Console.WriteLine("Comment is correctly placed in column " + commentColumn);
                }
                
                // احفظ المصنف
                workbook.Save("ThreadedCommentColumnDemo.xlsx");
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


