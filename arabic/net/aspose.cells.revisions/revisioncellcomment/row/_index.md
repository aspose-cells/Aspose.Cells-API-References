---
title: "RevisionCellComment.Row"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionCellComment. يحصل على فهرس الصف الذي يحتوي على تعليق"
type: docs
url: /ar/net/aspose.cells.revisions/revisioncellcomment/row/
---
## RevisionCellComment.Row property

يحصل على فهرس الصف الذي يحتوي على تعليق

```csharp
public int Row { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyRowDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد مع تتبع المراجعات
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف تعليقًا إلى الخلية D4 (الصف 3، العمود 3)
            int commentRow = 3;
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
                    
                    // اعرض قيمة خاصية Row
                    Console.WriteLine("Comment is located at row: " + commentRevision.Row);
                    
                    // أظهر استخدام خاصية Row
                    Console.WriteLine("Comment location details:");
                    Console.WriteLine("Row index: " + commentRevision.Row);
                    Console.WriteLine("Column index: " + commentRevision.Column);
                    Console.WriteLine("Cell name: " + commentRevision.CellName);
                    
                    // أظهر أن Row للقراءة فقط بمحاولة تعديلها (سيتسبب في خطأ تجميعي)
                    // commentRevision.Row = 5; // تم التعليق على هذا السطر لأن Row للقراءة فقط
                    
                    // طريقة بديلة لتغيير الموقع عن طريق تعديل CellName
                    Console.WriteLine("\nChanging comment position via CellName...");
                    commentRevision.CellName = "F10"; // Changes to row 9, column 5
                    Console.WriteLine("New Row index: " + commentRevision.Row);
                    Console.WriteLine("New Column index: " + commentRevision.Column);
                }
            }

            // احفظ المصنف مع التعديلات
            workbook.Save("RevisionCellCommentPropertyRowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


