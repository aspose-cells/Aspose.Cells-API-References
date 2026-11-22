---
title: "الفئة RevisionLog"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Revisions.RevisionLog فئة. تمثل سجل المراجعة"
type: docs
url: /ar/net/aspose.cells.revisions/revisionlog/
---
## RevisionLog class

يمثل سجل المراجعات.

```csharp
public class RevisionLog
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [MetadataTable](../../aspose.cells.revisions/revisionlog/metadatatable/) { get; } | يحصل على الجدول الذي يحتوي على بيانات التعريف حول قائمة من التغييرات المحددة التي حدثت لهذا دفتر العمل. |
| [Revisions](../../aspose.cells.revisions/revisionlog/revisions/) { get; } | يحصل على جميع المراجعات في هذا السجل. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionLogDemo
    {
        public static void RevisionLogExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook("HighlightedChangesWorkbook_original.xlsx");

            // الوصول إلى سجلات المراجعة لدفتر العمل
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // تحقق مما إذا كان هناك أي سجلات مراجعة
            if (revisionLogs.Count > 0)
            {
                // الوصول إلى سجل المراجعة الأول
                RevisionLog revisionLog = revisionLogs[0];

                // الوصول إلى جدول بيانات التعريف لسجل المراجعة
                RevisionHeader metadataTable = revisionLog.MetadataTable;

                // الوصول إلى المراجعات في سجل المراجعة
                RevisionCollection revisions = revisionLog.Revisions;

                // عرض بعض المعلومات حول المراجعات
                Console.WriteLine("Number of revisions: " + revisions.Count);
                Console.WriteLine("Metadata Table: " + metadataTable.ToString());
            }
            else
            {
                Console.WriteLine("No revision logs found.");
            }

            // احفظ المصنف
            workbook.Save("RevisionLogExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


