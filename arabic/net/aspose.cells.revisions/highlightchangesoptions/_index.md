---
title: "الفئة HighlightChangesOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Revisions.HighlightChangesOptions الفئة. تمثل خيارات تمييز المراجعات أو التغييرات في ملفات Excel المشتركة"
type: docs
url: /ar/net/aspose.cells.revisions/highlightchangesoptions/
---
## HighlightChangesOptions class

يمثل خيارات تمييز المراجعات أو التغييرات في ملفات إكسل المشتركة.

```csharp
public class HighlightChangesOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [HighlightChangesOptions](highlightchangesoptions/)(bool, bool) | يمثل خيارات تمييز المراجعات أو التغييرات في ملفات إكسل المشتركة. |

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;

namespace AsposeCellsExamples
{
    public class HighlightChangesOptionsDemo
    {
        public static void HighlightChangesExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook("HighlightedChangesWorkbook_original.xlsx");

            // احصل على سجلات المراجعات
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // حدد عدد الأيام للحفاظ على السجل التاريخي
            revisionLogs.DaysPreservingHistory = 30;

            // أنشئ HighlightChangesOptions
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);

            // تمييز التغييرات
            revisionLogs.HighlightChanges(options);

            // احفظ دفتر العمل مع التغييرات المميزة
            workbook.Save("HighlightedChangesWorkbook.xlsx");
            workbook.Save("HighlightedChangesWorkbook.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


