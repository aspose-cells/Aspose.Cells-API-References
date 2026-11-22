---
title: "Revision.Id"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Revision. يحصل على رقم هذا الإصدار"
type: docs
url: /ar/net/aspose.cells.revisions/revision/id/
---
## Revision.Id property

يحصل على رقم هذه المراجعة.

```csharp
public int Id { get; }
```

### ملاحظات

الصفر يعني أن هذا revision لا يحتوي على معرف.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionPropertyIdDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // قم بإجراء تغيير قد يؤدي إلى إنشاء revision
            worksheet.Cells["A1"].Value = "Sample Data";
            
            try
            {
                // احصل على مجموعة سجلات revision
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                
                if (revisionLogs != null && revisionLogs.Count > 0)
                {
                    // احصل على revisions من السجل الأول
                    RevisionCollection revisions = revisionLogs[0].Revisions;
                    
                    if (revisions != null && revisions.Count > 0)
                    {
                        // الوصول إلى revision الأول
                        Revision revision = revisions[0];
                        
                        // اعرض خاصية Id (للقراءة فقط)
                        Console.WriteLine("Revision Id: " + revision.Id);
                        
                        // احفظ المصنف
                        workbook.Save("RevisionIdDemo.xlsx");
                    }
                    else
                    {
                        Console.WriteLine("No revisions found in the log");
                    }
                }
                else
                {
                    Console.WriteLine("No revision logs were created");
                }
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

* class [Revision](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


