---
title: "Enum RevisionActionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Revisions.RevisionActionType enum. يمثل نوع إجراء المراجعة"
type: docs
url: /ar/net/aspose.cells.revisions/revisionactiontype/
---
## RevisionActionType enumeration

يمثل نوع إجراء المراجعة.

```csharp
public enum RevisionActionType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Add | `0` | إضافة مراجعة. |
| Delete | `1` | حذف مراجعة. |
| DeleteColumn | `2` | مراجعة حذف العمود. |
| DeleteRow | `3` | مراجعة حذف الصف. |
| InsertColumn | `4` | مراجعة إدراج العمود. |
| InsertRow | `5` | مراجعة إدراج الصف. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionActionTypeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد مع تتبع المراجعات
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تنفيذ عمليات مختلفة تُنتج أنواع مراجعات مختلفة
            worksheet.Cells["A1"].PutValue("Initial Value");
            worksheet.Cells.InsertRow(0);
            worksheet.Cells.DeleteRow(1);
            worksheet.Cells.InsertColumn(0);
            worksheet.Cells.DeleteColumn(1);

            // تحقق مما إذا كان المصنف يحتوي على مراجعات
            if (workbook.HasRevisions)
            {
                // ملاحظة: لا توفر واجهة برمجة التطبيقات الأصلية وصولًا مباشرًا إلى مجموعة المراجعات
                // لذا سنقوم فقط بعرض enum RevisionActionType كما هو مطلوب
                Console.WriteLine("Workbook contains revisions (but API doesn't provide access)");
            }

            // عرض استخدام قيم enum RevisionActionType
            Console.WriteLine("Available revision action types:");
            foreach (RevisionActionType actionType in Enum.GetValues(typeof(RevisionActionType)))
            {
                Console.WriteLine($"{actionType} = {(int)actionType}");
            }

            // احفظ المصنف
            workbook.Save("RevisionActionTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


