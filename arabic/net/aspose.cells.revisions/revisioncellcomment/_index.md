---
title: "الفئة RevisionCellComment"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Revisions.RevisionCellComment. تمثل سجل تعديل لتغيير تعليق الخلية"
type: docs
url: /ar/net/aspose.cells.revisions/revisioncellcomment/
---
## RevisionCellComment class

يمثل سجل مراجعة لتغيير تعليق خلية.

```csharp
public class RevisionCellComment : Revision
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioncellcomment/actiontype/) { get; } | يحصل على نوع الإجراء للمراجعة. |
| [CellName](../../aspose.cells.revisions/revisioncellcomment/cellname/) { get; set; } | يحصل على اسم الخلية. |
| [Column](../../aspose.cells.revisions/revisioncellcomment/column/) { get; } | يحصل على فهرس العمود الذي يحتوي على تعليق |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | يحصل على رقم هذه المراجعة.(موروث من [`Revision`](../revision/).) |
| [IsOldComment](../../aspose.cells.revisions/revisioncellcomment/isoldcomment/) { get; } | يشير إلى ما إذا كان التعليق قديمًا |
| [NewLength](../../aspose.cells.revisions/revisioncellcomment/newlength/) { get; } | يحصل على طول التعليق قبل إجراء هذا التعديل |
| [OldLength](../../aspose.cells.revisions/revisioncellcomment/oldlength/) { get; } | يحصل على طول نص التعليق المضاف في هذا التعديل |
| [Row](../../aspose.cells.revisions/revisioncellcomment/row/) { get; } | يحصل على فهرس الصف الذي يحتوي على تعليق |
| override [Type](../../aspose.cells.revisions/revisioncellcomment/type/) { get; } | يحصل على نوع المراجعة. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | يحصل على ورقة العمل. (موروث من [`Revision`](../revision/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionCellCommentDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد مع تتبع المراجعات
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف التعليق الأولي إلى الخلية A1
            Comment comment = worksheet.Comments[0, 0];
            comment.Note = "Initial comment text";

            // عدّل التعليق لإنشاء تعديل
            comment.Note = "Updated comment with more text";

            // الوصول إلى سجل التعديلات
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;

                    // عرض خصائص التعديل
                    Console.WriteLine("Revision Type: " + commentRevision.Type);
                    Console.WriteLine("Action Type: " + commentRevision.ActionType);
                    Console.WriteLine("Cell Location: " + commentRevision.CellName);
                    Console.WriteLine("Row: " + commentRevision.Row);
                    Console.WriteLine("Column: " + commentRevision.Column);

                    // إظهار تغييرات طول التعليق
                    Console.WriteLine("Old Length: " + commentRevision.OldLength);
                    Console.WriteLine("New Length: " + commentRevision.NewLength);
                    Console.WriteLine("Is Old Comment: " + commentRevision.IsOldComment);

                    // عدّل اسم الخلية لتوضيح تغيير الخاصية
                    string originalCellName = commentRevision.CellName;
                    commentRevision.CellName = "B2";
                    Console.WriteLine("Modified Cell Location: " + commentRevision.CellName);
                    Console.WriteLine("New Row: " + commentRevision.Row);
                    Console.WriteLine("New Column: " + commentRevision.Column);

                    // استعادة اسم الخلية الأصلي
                    commentRevision.CellName = originalCellName;
                }
            }

            // احفظ المصنف مع التعديلات
            workbook.Save("RevisionsClassRevisionCellCommentDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


