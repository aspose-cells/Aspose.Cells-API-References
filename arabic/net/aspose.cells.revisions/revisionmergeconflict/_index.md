---
title: "الفئة RevisionMergeConflict"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Revisions.RevisionMergeConflict فئة. تمثل سجل مراجعة يشير إلى حدوث تعارض دمج"
type: docs
url: /ar/net/aspose.cells.revisions/revisionmergeconflict/
---
## RevisionMergeConflict class

يمثل سجل مراجعة يشير إلى وجود تعارض دمج.

```csharp
public class RevisionMergeConflict : Revision
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | يحصل على رقم هذه المراجعة.(موروث من [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisionmergeconflict/type/) { get; } | يحصل على نوع المراجعة. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | يحصل على ورقة العمل. (موروث من [`Revision`](../revision/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionsClassRevisionMergeConflictDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // قم ببعض التغييرات لإنشاء تاريخ مراجعة
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A2"].PutValue("Another Value");

            // احفظ دفتر العمل لتوليد المراجعات
            workbook.Save("RevisionMergeConflictDemo_Before.xlsx");

            // إنشاء سيناريو تعارض دمج
            worksheet.Cells["A1"].PutValue("Conflicting Change 1");
            worksheet.Cells["A1"].PutValue("Conflicting Change 2");

            // احصل على تاريخ المراجعة (تكرار مباشرة عبر RevisionLogCollection)
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // ابحث ووضح RevisionMergeConflict
            foreach (RevisionLog revisionLog in revisionLogs)
            {
                foreach (Revision revision in revisionLog.Revisions)
                {
                    if (revision is RevisionMergeConflict mergeConflict)
                    {
                        // عرض الوصول إلى نوع المراجعة
                        RevisionType revisionType = mergeConflict.Type;
                    }
                }
            }

            // احفظ المصنف مع التعديلات
            workbook.Save("RevisionMergeConflictDemo_After.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


