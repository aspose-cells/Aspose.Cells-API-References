---
title: "RevisionInsertDelete.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionInsertDelete. تمثل نوع المراجعة"
type: docs
url: /ar/net/aspose.cells.revisions/revisioninsertdelete/type/
---
## RevisionInsertDelete.Type property

يمثل نوع المراجعة.

```csharp
public override RevisionType Type { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertDeletePropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد وتمكين تتبع المراجعات
            Workbook workbook = new Workbook();
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 30; // Enable revision tracking by setting days

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إدراج صف لإنشاء سجل مراجعة
            worksheet.Cells.InsertRows(0, 1);

            // احصل على مجموعة المراجعات (RevisionLogCollection نفسها هي المجموعة)
            RevisionLogCollection revisions = workbook.Worksheets.RevisionLogs;

            // ابحث عن RevisionInsertDelete في المراجعات
            foreach (RevisionLog revisionLog in revisions)
            {
                foreach (Revision revision in revisionLog.Revisions)
                {
                    if (revision is RevisionInsertDelete)
                    {
                        RevisionInsertDelete revisionInsertDelete = (RevisionInsertDelete)revision;

                        // عرض قيمة خاصية Type
                        Console.WriteLine("Revision Type: " + revisionInsertDelete.Type);

                        // عرض استخدام خاصية Type
                        if (revisionInsertDelete.Type == RevisionType.InsertDelete)
                        {
                            Console.WriteLine("This revision represents an insert/delete operation");
                            Console.WriteLine("Affected cell area: " + revisionInsertDelete.CellArea);
                            Console.WriteLine("Action type: " + revisionInsertDelete.ActionType);
                        }

                        break;
                    }
                }
            }

            // احفظ المصنف مع التعديلات
            workbook.Save("RevisionInsertDeletePropertyTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [RevisionType](../../revisiontype/)
* class [RevisionInsertDelete](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


