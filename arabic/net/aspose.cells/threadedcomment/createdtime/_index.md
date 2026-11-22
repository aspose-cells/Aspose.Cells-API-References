---
title: "ThreadedComment.CreatedTime"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreadedComment. تحصل وتعيّن وقت الإنشاء لهذا التعليق المتسلسل"
type: docs
url: /ar/net/aspose.cells/threadedcomment/createdtime/
---
## ThreadedComment.CreatedTime property

يحصل ويضبط وقت الإنشاء لهذا التعليق المتسلسل.

```csharp
public DateTime CreatedTime { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentPropertyCreatedTimeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء مؤلف تعليق متسلسل
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors["User1"];
            
            // إضافة تعليق إلى الخلية A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // إضافة تعليق متسلسل
            int threadedCommentIndex = comment.ThreadedComments.Add("Test comment", author);
            ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
            
            // إظهار خاصية CreatedTime
            Console.WriteLine("Threaded comment created at: " + threadedComment.CreatedTime);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


