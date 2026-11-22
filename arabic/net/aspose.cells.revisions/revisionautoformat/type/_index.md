---
title: "RevisionAutoFormat.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionAutoFormat. تحصل على نوع المراجعة"
type: docs
url: /ar/net/aspose.cells.revisions/revisionautoformat/type/
---
## RevisionAutoFormat.Type property

يحصل على نوع المراجعة.

```csharp
public override RevisionType Type { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionAutoFormatPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد مع تتبع المراجعات
            Workbook workbook = new Workbook();

            try
            {
                // الوصول إلى مجموعة سجلات المراجعة
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                
                // ابحث عن أول نسخة من RevisionAutoFormat
                RevisionAutoFormat revisionFormat = null;
                foreach (RevisionLog revisionLog in revisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionAutoFormat)
                        {
                            revisionFormat = (RevisionAutoFormat)revision;
                            break;
                        }
                    }
                    if (revisionFormat != null) break;
                }

                if (revisionFormat != null)
                {
                    // عرض خاصية Type (للقراءة فقط)
                    RevisionType type = revisionFormat.Type;
                    Console.WriteLine($"Revision type: {type}");
                    
                    // اعرض قيمة enum للتوضيح
                    Console.WriteLine($"Revision type value: {(int)type}");
                }
                else
                {
                    Console.WriteLine("No auto-format revisions found in the workbook");
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionAutoFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


