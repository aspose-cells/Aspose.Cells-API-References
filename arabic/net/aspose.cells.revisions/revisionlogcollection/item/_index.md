---
title: "RevisionLogCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionLogCollection. تحصل على RevisionLog حسب الفهرس"
type: docs
url: /ar/net/aspose.cells.revisions/revisionlogcollection/item/
---
## RevisionLogCollection indexer

يحصل على [`RevisionLog`](../../revisionlog/) حسب الفهرس.

```csharp
public RevisionLog this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس. |

### قيمة الإرجاع

يرجع كائن [`RevisionLog`](../../revisionlog/).

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionLogCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // فعّل المصنف المشترك لدعم التعديلات
            workbook.Settings.Shared = true;

            // الوصول إلى مجموعة سجلات المراجعة
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            try
            {
                // تحقق مما إذا كان هناك أي سجلات مراجعة
                if (revisionLogs.Count > 0)
                {
                    // الوصول إلى سجل التعديل الأول باستخدام خاصية Item
                    RevisionLog firstLog = revisionLogs[0];

                    // اعرض المعلومات الأساسية حول سجل التعديل
                    Console.WriteLine("First revision log accessed via Item property:");
                    Console.WriteLine($"Revision count: {firstLog.Revisions.Count}");
                }
                else
                {
                    Console.WriteLine("No revision logs available in the workbook.");
                }

                // احفظ المصنف
                workbook.Save("RevisionLogItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [RevisionLog](../../revisionlog/)
* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


