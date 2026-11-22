---
title: "Revision.Worksheet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Revision. يحصل على ورقة العمل"
type: docs
url: /ar/net/aspose.cells.revisions/revision/worksheet/
---
## Revision.Worksheet property

يحصل على ورقة العمل.

```csharp
public Worksheet Worksheet { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionPropertyWorksheetDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ضبط خصائص ورقة العمل
            worksheet.Name = "Demo Sheet";
            worksheet.IsGridlinesVisible = true;
            worksheet.DisplayZeros = false;
            worksheet.Zoom = 120;
            
            // إضافة بعض البيانات لتوضيح التنقيحات
            worksheet.Cells["A1"].PutValue("Original Value");
            
            // حماية ورقة العمل لتمكين تتبع التغييرات
            worksheet.Protect(ProtectionType.All);
            
            // إجراء تغيير سيتم تتبعه كتنقيح
            worksheet.Cells["A1"].PutValue("Modified Value");
            
            // حفظ دفتر عمل لتتبع التنقيحات
            workbook.Save("RevisionDemo.xlsx");
            
            // تحميل دفتر عمل مع التنقيحات
            Workbook workbookWithRevisions = new Workbook("RevisionDemo.xlsx");
            
            // الوصول إلى سجلات التنقيحات
            foreach (RevisionLog log in workbookWithRevisions.Worksheets.RevisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    // إظهار الوصول إلى خاصية Worksheet من التنقيح
                    Console.WriteLine($"Revision Type: {revision.Type}");
                    Console.WriteLine($"Worksheet Name: {revision.Worksheet.Name}");
                    Console.WriteLine($"Worksheet Index: {revision.Worksheet.Index}");
                    
                    if (revision.Type == RevisionType.ChangeCells)
                    {
                        RevisionCellChange cellChange = (RevisionCellChange)revision;
                        Console.WriteLine($"Cell changed in worksheet '{cellChange.Worksheet.Name}': {cellChange.CellName}");
                    }
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Revision](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


