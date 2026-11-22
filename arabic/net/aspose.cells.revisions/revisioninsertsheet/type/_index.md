---
title: "RevisionInsertSheet.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionInsertSheet. تُرجع نوع المراجعة"
type: docs
url: /ar/net/aspose.cells.revisions/revisioninsertsheet/type/
---
## RevisionInsertSheet.Type property

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

    public class RevisionInsertSheetPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد مع تتبع المراجعات
            Workbook workbook = new Workbook();
            
            // تمكين تتبع المراجعات (محاكاة لأن StartTrackingRevisions غير متوفر)
            bool trackRevisions = true;

            // أضف ورقة عمل جديدة لإنشاء سجل مراجعة
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
            
            // محاكاة الحصول على المراجعات (نظرًا لأن خاصية Revisions غير متوفرة)
            if (trackRevisions && workbook.HasRevisions)
            {
                // في سيناريو حقيقي، كنا سنصل إلى المراجعات هنا
                // هذا يفترض أننا حصلنا على المراجعة من مكان ما (مثل workbook.Revisions)
                RevisionInsertSheet insertSheetRevision = null; // Would be assigned from actual revisions collection
                
                if (insertSheetRevision != null)
                {
                    // اعرض خاصية Type
                    Console.WriteLine("Revision Type: " + insertSheetRevision.Type);

                    // أظهر استخدام خاصية Type للقراءة فقط
                    if (insertSheetRevision.Type == RevisionType.InsertSheet)
                    {
                        Console.WriteLine("This revision represents a sheet insertion operation");
                        
                        // اعرض معلومات إضافية حول الورقة المدخلة
                        Console.WriteLine("Inserted sheet name: " + insertSheetRevision.Name);
                        Console.WriteLine("Sheet position: " + insertSheetRevision.SheetPosition);
                    }

                    // تحقق مقابل أنواع مراجعات أخرى
                    if (insertSheetRevision.Type != RevisionType.Unknown)
                    {
                        Console.WriteLine("This is a known revision type");
                    }
                }

                // احفظ المصنف
                workbook.Save("RevisionInsertSheetTypeDemo.xlsx");
            }
            else
            {
                Console.WriteLine("No revisions found or revision tracking not enabled");
            }
        }
    }
}
```

### انظر أيضًا

* enum [RevisionType](../../revisiontype/)
* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


