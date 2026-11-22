---
title: "RevisionCellComment.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionCellComment. تحصل على نوع المراجعة"
type: docs
url: /ar/net/aspose.cells.revisions/revisioncellcomment/type/
---
## RevisionCellComment.Type property

يحصل على نوع المراجعة.

```csharp
public override RevisionType Type { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تعليق إلى الخلية A1
            int commentRow = 0;
            int commentCol = 0;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Initial comment";

            // تتبع المراجعات - تم التغيير لاستخدام خاصية HasRevisions
            // ملاحظة: في الاستخدام الفعلي، قد تحتاج إلى تمكين التتبع بوسائل أخرى
            // نظرًا لأن HasRevisions هي خاصية للقراءة فقط تشير إلى ما إذا كانت المراجعات موجودة

            // عدّل التعليق لإنشاء تعديل
            comment.Note = "Modified comment";

            // الوصول إلى المراجعات عبر مجموعة RevisionLogs الخاصة بـ Workbook
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // عرض قيمة خاصية Type
                    Console.WriteLine("Revision Type: " + commentRevision.Type);
                    
                    // عرض استخدام خاصية Type
                    if (commentRevision.Type == RevisionType.Comment)
                    {
                        Console.WriteLine("This revision is related to a comment change");
                        Console.WriteLine("Comment was modified at row: " + commentRevision.Row + ", column: " + commentRevision.Column);
                        Console.WriteLine("Old comment length: " + commentRevision.OldLength);
                        Console.WriteLine("New comment length: " + commentRevision.NewLength);
                    }
                }
            }

            // احفظ المصنف مع التعديلات
            workbook.Save("RevisionCellCommentPropertyTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [RevisionType](../../revisiontype/)
* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


