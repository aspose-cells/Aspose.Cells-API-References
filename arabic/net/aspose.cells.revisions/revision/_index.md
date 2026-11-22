---
title: "Class Revision"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Revisions.Revision class. يمثل المراجعة"
type: docs
url: /ar/net/aspose.cells.revisions/revision/
---
## Revision class

يمثل المراجعة.

```csharp
public abstract class Revision
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | يحصل على رقم هذه المراجعة. |
| virtual [Type](../../aspose.cells.revisions/revision/type/) { get; } | يمثل نوع المراجعة. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | يحصل على ورقة العمل. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // أضف بعض البيانات قد تُنشئ مراجعات
                worksheet.Cells["A1"].PutValue("Original Value");

                // احفظ المصنف لإنشاء خط أساس
                workbook.Save("RevisionDemo_Baseline.xlsx");

                // حمّل المصنف وأجرِ تغييرًا
                Workbook modifiedWorkbook = new Workbook("RevisionDemo_Baseline.xlsx");
                modifiedWorkbook.Worksheets[0].Cells["A1"].PutValue("Modified Value");

                // تحقق مما إذا كان هناك أي سجلات مراجعة
                if (modifiedWorkbook.Worksheets.RevisionLogs.Count > 0)
                {
                    RevisionLog log = modifiedWorkbook.Worksheets.RevisionLogs[0];
                    if (log.Revisions.Count > 0)
                    {
                        // احصل على أول مراجعة
                        Revision revision = log.Revisions[0];

                        // عرض الخصائص للقراءة فقط
                        Console.WriteLine($"Revision ID: {revision.Id}");
                        Console.WriteLine($"Revision Type: {revision.Type}");
                        Console.WriteLine($"Worksheet Name: {revision.Worksheet.Name}");

                        // احفظ المصنف المعدل
                        modifiedWorkbook.Save("RevisionDemo_Modified.xlsx");
                    }
                    else
                    {
                        Console.WriteLine("No revisions found in the log");
                    }
                }
                else
                {
                    Console.WriteLine("No revision logs available");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with Revision: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


