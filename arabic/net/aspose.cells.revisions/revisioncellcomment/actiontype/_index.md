---
title: "RevisionCellComment.ActionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionCellComment. تحصل على نوع الإجراء للمراجعة"
type: docs
url: /ar/net/aspose.cells.revisions/revisioncellcomment/actiontype/
---
## RevisionCellComment.ActionType property

يحصل على نوع الإجراء للمراجعة.

```csharp
public RevisionActionType ActionType { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyActionTypeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد مع تتبع المراجعات
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تعليق إلى الخلية A1
            Comment comment = worksheet.Comments[0, 0];
            comment.Note = "Initial comment";

            // عدّل التعليق لإنشاء تعديل
            comment.Note = "Updated comment";

            // أضف تعليقًا جديدًا لإنشاء مراجعة Add
            Comment newComment = worksheet.Comments[1, 1];
            newComment.Note = "New comment";

            // الوصول إلى revisions
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // عرض قيمة خاصية ActionType
                    Console.WriteLine("Revision ActionType: " + commentRevision.ActionType);
                    
                    // عرض استخدام خاصية ActionType
                    switch (commentRevision.ActionType)
                    {
                        case RevisionActionType.Add:
                            Console.WriteLine("This revision added a new comment at " + commentRevision.CellName);
                            break;
                        case RevisionActionType.Delete:
                            Console.WriteLine("This revision deleted a comment from " + commentRevision.CellName);
                            break;
                        default:
                            Console.WriteLine("This revision modified a comment at " + commentRevision.CellName);
                            break;
                    }

                    // اعرض الخصائص ذات الصلة
                    Console.WriteLine("Comment location: " + commentRevision.CellName);
                    Console.WriteLine("Is old comment: " + commentRevision.IsOldComment);
                    Console.WriteLine("Old length: " + commentRevision.OldLength);
                    Console.WriteLine("New length: " + commentRevision.NewLength);
                }
            }

            // احفظ المصنف مع التعديلات
            workbook.Save("RevisionCellCommentPropertyActionTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


