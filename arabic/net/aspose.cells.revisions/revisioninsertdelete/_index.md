---
title: "الفئة RevisionInsertDelete"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Revisions.RevisionInsertDelete. تمثل سجل تعديل لإجراء إدراج/حذف صف/عمود"
type: docs
url: /ar/net/aspose.cells.revisions/revisioninsertdelete/
---
## RevisionInsertDelete class

يمثل سجل مراجعة لإجراء إدراج/حذف صف/عمود.

```csharp
public class RevisionInsertDelete : Revision
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioninsertdelete/actiontype/) { get; } | يحصل على نوع الإجراء لهذا التعديل. |
| [CellArea](../../aspose.cells.revisions/revisioninsertdelete/cellarea/) { get; } | يحصل على نطاق الإدراج/الحذف. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | يحصل على رقم هذه المراجعة.(موروث من [`Revision`](../revision/).) |
| [Revisions](../../aspose.cells.revisions/revisioninsertdelete/revisions/) { get; } | يحصل على قائمة التعديلات بواسطة هذه العملية. |
| override [Type](../../aspose.cells.revisions/revisioninsertdelete/type/) { get; } | يمثل نوع المراجعة. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | يحصل على ورقة العمل. (موروث من [`Revision`](../revision/).) |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionsClassRevisionInsertDeleteDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;

            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells.InsertRow(0);
            worksheet.Cells.DeleteColumn(0);

            string filePath = "RevisionsDemo.xlsx";
            workbook.Save(filePath);

            Workbook reopenedWorkbook = new Workbook(filePath);
            foreach (RevisionLog log in reopenedWorkbook.Worksheets.RevisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision.Type == RevisionType.InsertDelete)
                    {
                        RevisionInsertDelete rid = (RevisionInsertDelete)revision;
                        Console.WriteLine($"ActionType: {rid.ActionType}, CellArea: {rid.CellArea}");
                    }
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


