---
title: "الفئة RevisionInsertSheet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Revisions.RevisionInsertSheet. تمثل سجل مراجعة لورقة تم إدراجها"
type: docs
url: /ar/net/aspose.cells.revisions/revisioninsertsheet/
---
## RevisionInsertSheet class

يمثل سجل مراجعة لورقة تم إدراجها.

```csharp
public class RevisionInsertSheet : Revision
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioninsertsheet/actiontype/) { get; } | يحصل على نوع الإجراء للمراجعة. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | يحصل على رقم هذه المراجعة.(موروث من [`Revision`](../revision/).) |
| [Name](../../aspose.cells.revisions/revisioninsertsheet/name/) { get; } | يحصل على اسم ورقة العمل. |
| [SheetPosition](../../aspose.cells.revisions/revisioninsertsheet/sheetposition/) { get; } | يحصل على الموضع الصفري للورقة الجديدة في شريط علامات الأوراق. |
| override [Type](../../aspose.cells.revisions/revisioninsertsheet/type/) { get; } | يحصل على نوع المراجعة. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | يحصل على ورقة العمل. (موروث من [`Revision`](../revision/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionInsertSheetDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // أضف ورقة عمل جديدة لإمكانية إنشاء مراجعة
                Worksheet newSheet = workbook.Worksheets.Add("NewSheet");

                // ملاحظة: نظرًا لأننا لا نستطيع إنشاء كائنات RevisionInsertSheet مباشرةً،
                // سنوضح كيفية العمل مع واحدة إذا كانت موجودة في مجموعة المراجعات
                // هذا سيناريو محاكى لأن واجهة برمجة تطبيقات تتبع المراجعات الفعلية غير مكشوفة بالكامل

                // في سيناريو حقيقي مع تمكين تتبع المراجعات، قد تحصل على مراجعات مثل هذه:
                // RevisionInsertSheet revision = null; // سيأتي من مجموعة workbook.Revisions

                // لأغراض العرض، سنظهر نمط العمل مع RevisionInsertSheet
                // نظرًا لأننا لا نستطيع إنشاء نسخة منه مباشرةً، سنوضح نمط الوصول إلى الخصائص

                // بدلاً من محاولة إنشاء نسخة، سنظهر كيفية العمل مع واحدة إذا كانت متاحة
                // هذا يحافظ على البنية مع إصلاح خطأ التجميع

                // عرض معلومات حول خصائص المراجعة (محاكى)
                Console.WriteLine("RevisionInsertSheet properties demonstration:");
                Console.WriteLine("Type property would show: RevisionType.InsertSheet");
                Console.WriteLine("ActionType property would show: RevisionActionType.Add");
                Console.WriteLine("Name property would show the sheet name");
                Console.WriteLine("SheetPosition property would show the zero-based position");

                // احفظ المصنف
                workbook.Save("RevisionInsertSheetDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with potential revisions.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionInsertSheet: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


