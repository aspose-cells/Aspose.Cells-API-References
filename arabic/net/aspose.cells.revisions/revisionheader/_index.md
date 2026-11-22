---
title: "الفئة RevisionHeader"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Revisions.RevisionHeader فئة. تمثل قائمة بالتغييرات المحددة التي حدثت لهذا المصنف"
type: docs
url: /ar/net/aspose.cells.revisions/revisionheader/
---
## RevisionHeader class

يمثل قائمة بالتغييرات المحددة التي حدثت لهذا المصنف.

```csharp
public class RevisionHeader
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [RevisionHeader](revisionheader/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [SavedTime](../../aspose.cells.revisions/revisionheader/savedtime/) { get; set; } | يحصل ويضبط التاريخ والوقت عندما تم حفظ مجموعة المراجعات هذه. |
| [UserName](../../aspose.cells.revisions/revisionheader/username/) { get; set; } | يحصل ويضبط اسم المستخدم الذي يقوم بالمراجعة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionHeaderDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إنشاء نسخة من الفئة RevisionHeader
                RevisionHeader revisionHeader = new RevisionHeader();

                // ضبط الخصائص الأساسية
                revisionHeader.SavedTime = DateTime.Now;
                revisionHeader.UserName = "TestUser";

                // عرض الوظيفة الأساسية
                Console.WriteLine($"Revision saved by: {revisionHeader.UserName}");
                Console.WriteLine($"Revision saved at: {revisionHeader.SavedTime}");

                // احفظ المصنف
                workbook.Save("RevisionHeaderDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with revision header information.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionHeader: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


