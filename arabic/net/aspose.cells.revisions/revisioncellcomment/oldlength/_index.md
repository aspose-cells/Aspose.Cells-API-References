---
title: "RevisionCellComment.OldLength"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionCellComment. يحصل على طول نص التعليق المضاف في هذا revision"
type: docs
url: /ar/net/aspose.cells.revisions/revisioncellcomment/oldlength/
---
## RevisionCellComment.OldLength property

يحصل على طول نص التعليق المضاف في هذا التعديل

```csharp
public int OldLength { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyOldLengthDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد مع تتبع المراجعات
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف تعليقًا إلى الخلية D4
            int commentRow = 3;
            int commentCol = 3;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            string initialComment = "Original comment text";
            comment.Note = initialComment;

            // عدّل التعليق لإنشاء تعديل
            string updatedComment = "This is the modified comment text with more content";
            comment.Note = updatedComment;

            // الوصول إلى revisions
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // اعرض قيمة خاصية OldLength
                    Console.WriteLine("Old comment length: " + commentRevision.OldLength);
                    Console.WriteLine("Actual initial comment length: " + initialComment.Length);
                    
                    // اعرض الخصائص ذات الصلة
                    Console.WriteLine("New comment length: " + commentRevision.NewLength);
                    Console.WriteLine("Comment location: " + commentRevision.CellName);
                    
                    // أظهر استخدام خاصية OldLength
                    if (commentRevision.OldLength > 0)
                    {
                        Console.WriteLine("Comment existed before modification with length: " + 
                            commentRevision.OldLength);
                            
                        double expansionPercentage = ((double)(commentRevision.NewLength - commentRevision.OldLength) / 
                            commentRevision.OldLength) * 100;
                        Console.WriteLine($"Comment expanded by {expansionPercentage:F2}%");
                    }
                }
            }

            // احفظ المصنف مع التعديلات
            workbook.Save("RevisionCellCommentPropertyOldLengthDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


