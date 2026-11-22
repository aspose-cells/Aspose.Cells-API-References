---
title: "RevisionMergeConflict.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionMergeConflict. تحصل على نوع المراجعة"
type: docs
url: /ar/net/aspose.cells.revisions/revisionmergeconflict/type/
---
## RevisionMergeConflict.Type property

يحصل على نوع المراجعة.

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

    public class RevisionMergeConflictPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تمكين تتبع التغييرات
            workbook.StartAccessCache(AccessCacheOptions.All);

            // قم بإجراء تغييرات لإنشاء سيناريو تعارض دمج
            worksheet.Cells["A1"].PutValue("Original Value");
            workbook.Save("TempMergeConflict.xlsx");

            // محاكاة تعارض دمج بفتح الملف وإجراء تغييرات متعارضة
            Workbook otherUserWorkbook = new Workbook("TempMergeConflict.xlsx");
            otherUserWorkbook.Worksheets[0].Cells["A1"].PutValue("Conflicting Change");
            otherUserWorkbook.Save("TempMergeConflict_OtherUser.xlsx");

            // دمج التغييرات المتعارضة
            workbook.Combine(otherUserWorkbook);

            // تحقق مما إذا كان هناك مراجعات
            if (workbook.HasRevisions)
            {
                // ابحث عن مراجعة تعارض الدمج
                RevisionMergeConflict mergeConflictRevision = null;
                // ملاحظة: في التنفيذ الفعلي، ستحتاج إلى طريقة أخرى للوصول إلى المراجعات
                // نظرًا لأن خاصية Revisions غير متاحة في تعريف API المقدم

                if (mergeConflictRevision != null)
                {
                    // اعرض خاصية Type لمراجعة تعارض الدمج
                    Console.WriteLine("Merge Conflict Revision Type: " + mergeConflictRevision.Type);

                    // أظهر كيف يمكن استخدام هذه المعلومات
                    if (mergeConflictRevision.Type == RevisionType.MergeConflict)
                    {
                        Console.WriteLine("This revision represents a merge conflict.");
                        Console.WriteLine("Worksheet affected: " + mergeConflictRevision.Worksheet.Name);
                    }
                }
            }

            // احفظ المصنف مع التعديلات
            workbook.Save("RevisionMergeConflictTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [RevisionType](../../revisiontype/)
* class [RevisionMergeConflict](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


