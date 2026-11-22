---
title: "RevisionCustomView.ActionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionCustomView. تحصل على نوع الإجراء"
type: docs
url: /ar/net/aspose.cells.revisions/revisioncustomview/actiontype/
---
## RevisionCustomView.ActionType property

يحصل على نوع الإجراء.

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

    public class RevisionCustomViewPropertyActionTypeDemo
    {
        public static void Run()
        {
            try
            {
                // حمّل دفتر عمل موجود قد يحتوي على مراجعات عرض مخصص
                Workbook workbook = new Workbook("SampleWithRevisions.xlsx");

                // تكرار عبر جميع سجلات المراجعة في دفتر العمل
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    // تحقق من كل مراجعة في السجل
                    foreach (Revision revision in log.Revisions)
                    {
                        // تحقق مما إذا كانت هذه مراجعة عرض مخصص
                        if (revision is RevisionCustomView)
                        {
                            RevisionCustomView customViewRevision = (RevisionCustomView)revision;

                            // عرض قيمة خاصية ActionType
                            Console.WriteLine($"Custom View Revision Action Type: {customViewRevision.ActionType}");

                            // وضح كيفية استخدام خاصية ActionType
                            switch (customViewRevision.ActionType)
                            {
                                case RevisionActionType.Add:
                                    Console.WriteLine("This revision represents adding a custom view");
                                    break;
                                case RevisionActionType.Delete:
                                    Console.WriteLine("This revision represents deleting a custom view");
                                    break;
                                default:
                                    Console.WriteLine("This revision represents another type of action");
                                    break;
                            }

                            // اعرض خصائص إضافية للسياق
                            Console.WriteLine($"Revision Type: {customViewRevision.Type}");
                            Console.WriteLine($"Custom View GUID: {customViewRevision.Guid}");
                        }
                    }
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

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


