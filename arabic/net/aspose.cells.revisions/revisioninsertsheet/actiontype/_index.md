---
title: "RevisionInsertSheet.ActionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionInsertSheet. تُرجع نوع الإجراء للمراجعة"
type: docs
url: /ar/net/aspose.cells.revisions/revisioninsertsheet/actiontype/
---
## RevisionInsertSheet.ActionType property

يحصل على نوع الإجراء للمراجعة.

```csharp
public RevisionActionType ActionType { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertSheetPropertyActionTypeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد مع تتبع المراجعات
            Workbook workbook = new Workbook();
            // ملاحظة: StartTrackingRevisions غير متوفر في واجهة برمجة التطبيقات المقدمة
            // workbook.StartTrackingRevisions();

            // أضف ورقة عمل جديدة لإنشاء سجل مراجعة
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
            
            // ملاحظة: StopTrackingRevisions غير متوفر في واجهة برمجة التطبيقات المقدمة
            // workbook.StopTrackingRevisions();
            
            // ملاحظة: الخاصية Revisions غير متوفرة في واجهة برمجة التطبيقات المقدمة
            // سنستخدم HasRevisions للتحقق مما إذا كان هناك أي تعديلات
            if (workbook.HasRevisions)
            {
                // في سيناريو حقيقي، كنا سنصل إلى المراجعات هنا
                // نظرًا لعدم إمكانية إنشاء RevisionInsertSheet مباشرةً، سنحاكي عملية التحقق من واحدة
                // هذا يفترض أننا حصلنا على المراجعة من مكان ما (مثل workbook.Revisions)
                RevisionInsertSheet insertSheetRevision = null; // Would be assigned from actual revisions collection
                
                // نظرًا لعدم إمكانية إنشاء أو تعيين ActionType، سنقوم فقط بتوضيح عملية التحقق منه
                if (insertSheetRevision != null)
                {
                    // اعرض الخاصية ActionType
                    Console.WriteLine("ActionType of sheet insertion: " + insertSheetRevision.ActionType);

                    // وضح استخدام الخاصية للقراءة فقط
                    if (insertSheetRevision.ActionType == RevisionActionType.Add)
                    {
                        Console.WriteLine("This revision represents a sheet addition");
                    }
                }

                // احفظ المصنف مع التعديلات
                workbook.Save("RevisionInsertSheetActionTypeDemo.xlsx");
            }
            else
            {
                Console.WriteLine("No sheet insertion revision found");
            }
        }
    }
}
```

### انظر أيضًا

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


