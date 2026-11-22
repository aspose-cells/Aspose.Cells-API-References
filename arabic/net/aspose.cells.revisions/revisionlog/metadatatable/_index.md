---
title: "RevisionLog.MetadataTable"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionLog. تحصل على جدول يحتوي على بيانات تعريفية حول قائمة من التغييرات المحددة التي حدثت لهذا دفتر العمل"
type: docs
url: /ar/net/aspose.cells.revisions/revisionlog/metadatatable/
---
## RevisionLog.MetadataTable property

يحصل على الجدول الذي يحتوي على بيانات التعريف حول قائمة من التغييرات المحددة التي حدثت لهذا دفتر العمل.

```csharp
public RevisionHeader MetadataTable { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionLogPropertyMetadataTableDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // قم ببعض التغييرات لإنشاء تاريخ مراجعة
            worksheet.Cells["A1"].PutValue("Original Value");
            workbook.Save("RevisionDemo.xlsx", SaveFormat.Xlsx);
            
            // تعديل الخلية لإنشاء مراجعة
            worksheet.Cells["A1"].PutValue("Modified Value");
            workbook.Save("RevisionDemo_modified.xlsx", SaveFormat.Xlsx);

            // أعد فتح دفتر العمل المعدل للوصول إلى سجلات المراجعة
            workbook = new Workbook("RevisionDemo_modified.xlsx");
            
            // الوصول إلى سجلات التنقيحات
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            
            if (revisionLogs.Count > 0)
            {
                RevisionLog revisionLog = revisionLogs[0];
                RevisionHeader metadata = revisionLog.MetadataTable;
                
                Console.WriteLine("Revision Metadata:");
                Console.WriteLine("Saved Time: " + metadata.SavedTime);
                Console.WriteLine("Modified By: " + metadata.UserName);
                Console.WriteLine("Number of Revisions: " + revisionLog.Revisions.Count);
            }
            else
            {
                Console.WriteLine("No revision history found");
            }
        }
    }
}
```

### انظر أيضًا

* class [RevisionHeader](../../revisionheader/)
* class [RevisionLog](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


