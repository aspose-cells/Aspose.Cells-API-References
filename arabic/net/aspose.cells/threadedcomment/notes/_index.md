---
title: "ThreadedComment.Notes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreadedComment. تحصل وتعيّن نص التعليق"
type: docs
url: /ar/net/aspose.cells/threadedcomment/notes/
---
## ThreadedComment.Notes property

يحصل ويضبط نص التعليق.

```csharp
public string Notes { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentPropertyNotesDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إنشاء أو الحصول على مؤلف التعليق المتسلسل
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors["User1"];
                author.Name = "User1";

                // إضافة تعليق متسلسل إلى الخلية A1 (الصف 0، العمود 0) مع النص الأولي
                worksheet.Comments.AddThreadedComment(0, 0, "Initial comment text", author);

                // استرجاع التعليق المتسلسل المضاف حديثًا
                ThreadedComment threadedComment = worksheet.Comments[0].ThreadedComments[0];

                // تحديث خاصية Notes (نص التعليق)
                threadedComment.Notes = "Updated comment notes";

                // قراءة وعرض قيمة خاصية Notes
                Console.WriteLine("Threaded comment Notes: " + threadedComment.Notes);

                // احفظ دفتر العمل (اختياري)
                workbook.Save("ThreadedCommentNotesDemo.xlsx");
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


