---
title: "RevisionAutoFormat.CellArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionAutoFormat. تحصل على الموقع الذي تم تطبيق التنسيق فيه"
type: docs
url: /ar/net/aspose.cells.revisions/revisionautoformat/cellarea/
---
## RevisionAutoFormat.CellArea property

يحصل على الموقع الذي تم تطبيق التنسيق فيه.

```csharp
public CellArea CellArea { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionAutoFormatPropertyCellAreaDemo
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
                    // عرض خاصية CellArea (للقراءة فقط)
                    CellArea area = revisionFormat.CellArea;
                    Console.WriteLine($"Formatting applied to area: StartRow={area.StartRow}, " +
                                      $"StartColumn={area.StartColumn}, EndRow={area.EndRow}, " +
                                      $"EndColumn={area.EndColumn}");
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

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionAutoFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


