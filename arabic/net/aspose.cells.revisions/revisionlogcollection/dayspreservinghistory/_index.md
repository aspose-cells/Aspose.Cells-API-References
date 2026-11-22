---
title: "RevisionLogCollection.DaysPreservingHistory"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionLogCollection. تحصل وتعيّن عدد الأيام التي سيحتفظ فيها تطبيق الجداول الإلكترونية بسجل التغييرات لهذا المصنف"
type: docs
url: /ar/net/aspose.cells.revisions/revisionlogcollection/dayspreservinghistory/
---
## RevisionLogCollection.DaysPreservingHistory property

يحصل على ويضبط عدد الأيام التي سيحتفظ فيها تطبيق الجداول الإلكترونية بسجل التغييرات لهذا المصنف.

```csharp
public int DaysPreservingHistory { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RevisionLogCollectionPropertyDaysPreservingHistoryDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Value");
            
            // عيّن خاصية DaysPreservingHistory
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 40;
            
            string outputPath = "output_DaysPreservingHistory.xlsx";
            workbook.Save(outputPath);
            
            // أعد التحميل للتحقق من الخاصية
            Workbook loadedWorkbook = new Workbook(outputPath);
            Console.WriteLine("DaysPreservingHistory: " + 
                loadedWorkbook.Worksheets.RevisionLogs.DaysPreservingHistory);
        }
    }
}
```

### انظر أيضًا

* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


