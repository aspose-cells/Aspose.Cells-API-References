---
title: "RevisionHeader.SavedTime"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionHeader. تحصل وتضبط التاريخ والوقت عندما تم حفظ مجموعة المراجعات هذه"
type: docs
url: /ar/net/aspose.cells.revisions/revisionheader/savedtime/
---
## RevisionHeader.SavedTime property

يحصل ويضبط التاريخ والوقت عندما تم حفظ مجموعة المراجعات هذه.

```csharp
public DateTime SavedTime { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionHeaderPropertySavedTimeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أنشئ مثيلًا لـ RevisionHeader
            RevisionHeader revisionHeader = new RevisionHeader();
            
            try
            {
                // عيّن خاصية SavedTime
                revisionHeader.SavedTime = DateTime.Now;
                
                // احصل على قيمة SavedTime واعرضها
                Console.WriteLine("SavedTime value: " + revisionHeader.SavedTime);
                
                // عدّل خاصية SavedTime
                revisionHeader.SavedTime = DateTime.Now.AddHours(-1);
                Console.WriteLine("Modified SavedTime value: " + revisionHeader.SavedTime);
                
                // احفظ workbook لتوضيح أن الخاصية تُستخدم
                workbook.Save("SavedTimeDemo.xlsx");
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

* class [RevisionHeader](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


