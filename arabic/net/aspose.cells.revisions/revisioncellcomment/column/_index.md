---
title: "RevisionCellComment.Column"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionCellComment. تحصل على فهرس العمود الذي يحتوي على تعليق"
type: docs
url: /ar/net/aspose.cells.revisions/revisioncellcomment/column/
---
## RevisionCellComment.Column property

يحصل على فهرس العمود الذي يحتوي على تعليق

```csharp
public int Column { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف تعليقًا إلى الخلية D3
            int commentRow = 2;
            int commentCol = 3;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Sample comment for revision tracking";

            // عدّل التعليق لإنشاء تعديل
            comment.Note = "Updated comment text";

            // الوصول إلى revisions
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // اعرض قيمة خاصية Column
                    Console.WriteLine("Comment revision column index: " + commentRevision.Column);
                    
                    // أظهر طريقة استخدام خاصية Column
                    Console.WriteLine("Comment was modified in column: " + (char)('A' + commentRevision.Column));
                    
                    // اعرض الخصائص ذات الصلة
                    Console.WriteLine("Associated row: " + commentRevision.Row);
                    Console.WriteLine("Cell name: " + commentRevision.CellName);
                    
                    // ملاحظة: العمود للقراءة فقط، لذا لا يمكننا تعديلها مباشرة
                    // يمكننا تغييره بشكل غير مباشر عن طريق تعديل CellName
                    string originalCellName = commentRevision.CellName;
                    commentRevision.CellName = "E5"; // This will update both Row and Column properties
                    Console.WriteLine("After CellName change - New column: " + commentRevision.Column);
                    
                    // استرجع القيمة الأصلية
                    commentRevision.CellName = originalCellName;
                }
            }

            // احفظ المصنف مع التعديلات
            workbook.Save("RevisionCellCommentPropertyColumnDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


