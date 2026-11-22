---
title: "RevisionRenameSheet.NewName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionRenameSheet. تحصل على الاسم الجديد لورقة العمل"
type: docs
url: /ar/net/aspose.cells.revisions/revisionrenamesheet/newname/
---
## RevisionRenameSheet.NewName property

يحصل على الاسم الجديد للورقة.

```csharp
public string NewName { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionRenameSheetPropertyNewNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل وإعادة تسميتها لتفعيل مراجعة
            Worksheet sheet = workbook.Worksheets[0];
            string originalName = sheet.Name;
            string newName = "RenamedSheet";
            sheet.Name = newName;

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
                        Console.WriteLine("Sheet renamed from '{0}' to '{1}'", 
                            renameSheet.OldName, renameSheet.NewName);
                        
                        // عرض استخدام خاصية NewName
                        if (renameSheet.NewName == newName)
                        {
                            Console.WriteLine("NewName property verification successful");
                        }
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


