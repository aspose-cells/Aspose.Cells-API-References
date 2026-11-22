---
title: "RevisionLog.Revisions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionLog. تحصل على جميع المراجعات في هذا السجل"
type: docs
url: /ar/net/aspose.cells.revisions/revisionlog/revisions/
---
## RevisionLog.Revisions property

يحصل على جميع المراجعات في هذا السجل.

```csharp
public RevisionCollection Revisions { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionLogPropertyRevisionsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف مع سجل المراجعات
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // قم بإجراء بعض التغييرات لتتبع المراجعات
            worksheet.Cells["A1"].PutValue("Initial Value");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].Formula = "=A2*2";
            
            // احفظ مع تتبع المراجعات
            workbook.Save("revision_demo.xlsx", SaveFormat.Xlsx);
            
            // قم بإجراء مزيد من التغييرات لإنشاء مراجعات
            worksheet.Cells["A1"].PutValue("Modified Value");
            worksheet.Cells["A2"].PutValue(200);
            
            // احفظ مرة أخرى لتسجيل المراجعات
            workbook.Save("revision_demo.xlsx", SaveFormat.Xlsx);
            
            // تحميل دفتر عمل مع التنقيحات
            Workbook workbookWithRevisions = new Workbook("revision_demo.xlsx");
            
            // الوصول إلى سجلات التنقيحات
            RevisionLogCollection revisionLogs = workbookWithRevisions.Worksheets.RevisionLogs;
            
            // معالجة كل سجل مراجعات
            foreach (RevisionLog log in revisionLogs)
            {
                Console.WriteLine($"Processing revision log with {log.Revisions.Count} revisions");
                
                // الوصول إلى مجموعة المراجعات
                RevisionCollection revisions = log.Revisions;
                
                foreach (Revision revision in revisions)
                {
                    Console.WriteLine($"Revision Type: {revision.Type}");
                    
                    if (revision.Type == RevisionType.ChangeCells)
                    {
                        RevisionCellChange cellChange = (RevisionCellChange)revision;
                        Console.WriteLine($"Cell {cellChange.CellName} changed from '{cellChange.OldValue}' to '{cellChange.NewValue}'");
                    }
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [RevisionCollection](../../revisioncollection/)
* class [RevisionLog](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


