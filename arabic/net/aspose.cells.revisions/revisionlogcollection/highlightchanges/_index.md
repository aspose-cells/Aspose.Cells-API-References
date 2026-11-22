---
title: "RevisionLogCollection.HighlightChanges"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة RevisionLogCollection. تبرز التغييرات في المصنف المشترك"
type: docs
url: /ar/net/aspose.cells.revisions/revisionlogcollection/highlightchanges/
---
## RevisionLogCollection.HighlightChanges method

يسلط الضوء على تغييرات المصنف المشترك.

```csharp
public void HighlightChanges(HighlightChangesOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خيارات | HighlightChangesOptions | عيّن الخيارات لتصفية التغييرات التي يجب تتبعها. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionLogCollectionMethodHighlightChangesWithHighlightChangesOptionsDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض البيانات النموذجية والتعديلات
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A1"].PutValue("Modified Value");
            
            // تسليط الضوء على التغييرات مع الخيارات
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);
            workbook.Worksheets.RevisionLogs.HighlightChanges(options);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HighlightChangesOptions](../../highlightchangesoptions/)
* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


