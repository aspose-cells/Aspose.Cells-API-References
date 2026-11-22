---
title: "الفئة RevisionRenameSheet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Revisions.RevisionRenameSheet. تمثل تعديلًا لإعادة تسمية الورقة"
type: docs
url: /ar/net/aspose.cells.revisions/revisionrenamesheet/
---
## RevisionRenameSheet class

يمثل مراجعة لإعادة تسمية الورقة.

```csharp
public class RevisionRenameSheet : Revision
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | يحصل على رقم هذه المراجعة.(موروث من [`Revision`](../revision/).) |
| [NewName](../../aspose.cells.revisions/revisionrenamesheet/newname/) { get; } | يحصل على الاسم الجديد للورقة. |
| [OldName](../../aspose.cells.revisions/revisionrenamesheet/oldname/) { get; } | يحصل على الاسم القديم للورقة. |
| override [Type](../../aspose.cells.revisions/revisionrenamesheet/type/) { get; } | يمثل نوع المراجعة. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | يحصل على ورقة العمل. (موروث من [`Revision`](../revision/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionRenameSheetDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // احفظ الاسم الأصلي وأعد تسمية الورقة
                string originalName = worksheet.Name;
                worksheet.Name = "RenamedSheet";

                // احفظ إلى تدفق الذاكرة لإنشاء المراجعات
                System.IO.MemoryStream ms = new System.IO.MemoryStream();
                workbook.Save(ms, SaveFormat.Xlsx);

                // أعد فتح دفتر العمل للوصول إلى سجلات المراجعات
                workbook = new Workbook(ms);

                // تحقق من سجلات المراجعات لعملية إعادة التسمية
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision rv in log.Revisions)
                    {
                        if (rv.Type == RevisionType.RenameSheet)
                        {
                            RevisionRenameSheet renameSheet = (RevisionRenameSheet)rv;
                            Console.WriteLine("Revision Type: " + renameSheet.Type);
                            Console.WriteLine("Old Sheet Name: " + renameSheet.OldName);
                            Console.WriteLine("New Sheet Name: " + renameSheet.NewName);
                        }
                    }
                }

                // احفظ المصنف
                workbook.Save("RevisionRenameSheetDemo.xlsx");
                Console.WriteLine("RevisionRenameSheet demo completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in RevisionRenameSheet demo: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


