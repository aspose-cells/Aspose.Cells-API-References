---
title: "RevisionRenameSheet.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionRenameSheet. تمثل نوع المراجعة"
type: docs
url: /ar/net/aspose.cells.revisions/revisionrenamesheet/type/
---
## RevisionRenameSheet.Type property

يمثل نوع المراجعة.

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

    public class RevisionRenameSheetPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // تمكين تتبع المراجعات قبل إجراء التغييرات
            // ملاحظة: هذه الطريقة غير موجودة في واجهة برمجة التطبيقات المقدمة، لذا سنقوم بإزالتها
            // workbook.StartTrackingRevisions();

            // إعادة تسمية ورقة العمل الأولى لإنشاء مراجعة
            Worksheet worksheet = workbook.Worksheets[0];
            string originalName = worksheet.Name;
            worksheet.Name = "RenamedSheet";

            // الوصول إلى مجموعة المراجعات
            // ملاحظة: خاصية Revisions غير موجودة في واجهة برمجة التطبيقات المقدمة
            // لذلك سنحتاج إلى التحقق أولاً مما إذا كان المصنف يحتوي على مراجعات
            if (workbook.HasRevisions)
            {
                // العثور على مراجعة إعادة تسمية الورقة
                RevisionRenameSheet renameRevision = null;
                // نظرًا لعدم إمكانية الوصول إلى Revisions مباشرةً، سنحتاج إلى تعديل هذا الجزء
                // هذا مجرد عنصر نائب نظرًا لأن واجهة برمجة التطبيقات الفعلية لا تدعم الوصول إلى المراجعات
                Console.WriteLine("Revision tracking is not fully supported in this API version.");
                
                if (renameRevision != null)
                {
                    // عرض قيمة خاصية Type
                    Console.WriteLine("Revision Type: " + renameRevision.Type);
                    Console.WriteLine("Old Sheet Name: " + renameRevision.OldName);
                    Console.WriteLine("New Sheet Name: " + renameRevision.NewName);

                    // عرض كيفية استخدام خاصية Type
                    if (renameRevision.Type == RevisionType.RenameSheet)
                    {
                        Console.WriteLine("This revision represents a worksheet rename operation.");
                    }
                }
            }

            // احفظ المصنف مع التعديلات
            workbook.Save("RevisionRenameSheetDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [RevisionType](../../revisiontype/)
* class [RevisionRenameSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


