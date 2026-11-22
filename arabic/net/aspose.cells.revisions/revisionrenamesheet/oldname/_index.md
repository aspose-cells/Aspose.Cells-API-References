---
title: "RevisionRenameSheet.OldName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionRenameSheet. يحصل على الاسم القديم لورقة العمل"
type: docs
url: /ar/net/aspose.cells.revisions/revisionrenamesheet/oldname/
---
## RevisionRenameSheet.OldName property

يحصل على الاسم القديم للورقة.

```csharp
public string OldName { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionRenameSheetPropertyOldNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل وإعادة تسميتها لتفعيل مراجعة
            Worksheet sheet = workbook.Worksheets[0];
            string originalName = sheet.Name;
            sheet.Name = "RenamedSheet";

            // الوصول إلى سجلات المراجعة
            foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
            {
                foreach (Revision rv in log.Revisions)
                {
                    if (rv.Type == RevisionType.RenameSheet)
                    {
                        RevisionRenameSheet rsnm = (RevisionRenameSheet)rv;
                        Console.WriteLine("Sheet renamed from: {0} to: {1}", rsnm.OldName, rsnm.NewName);
                    }
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [RevisionRenameSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


