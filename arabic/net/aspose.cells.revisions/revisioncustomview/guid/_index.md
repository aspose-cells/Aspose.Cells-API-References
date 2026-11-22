---
title: "RevisionCustomView.Guid"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionCustomView. تحصل على المعرف الفريد عالميًا للعرض المخصص"
type: docs
url: /ar/net/aspose.cells.revisions/revisioncustomview/guid/
---
## RevisionCustomView.Guid property

يحصل على المعرف الفريد عالميًا للعرض المخصص.

```csharp
public Guid Guid { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionCustomViewPropertyGuidDemo
    {
        public static void Run()
        {
            // فتح مصنف موجود يحتوي على مراجعات عرض مخصص
            Workbook workbook = new Workbook("example.xlsx");
            
            // معالجة سجلات المراجعة
            foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision.Type == RevisionType.CustomView)
                    {
                        RevisionCustomView rcv = (RevisionCustomView)revision;
                        Console.WriteLine($"ActionType: {rcv.ActionType}, Guid: {rcv.Guid}");
                    }
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


