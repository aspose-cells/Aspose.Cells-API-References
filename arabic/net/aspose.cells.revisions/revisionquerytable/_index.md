---
title: "الفئة RevisionQueryTable"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Revisions.RevisionQueryTable. تمثل مراجعة لتغيير حقل جدول الاستعلام"
type: docs
url: /ar/net/aspose.cells.revisions/revisionquerytable/
---
## RevisionQueryTable class

يمثل مراجعة لتغيير حقل جدول الاستعلام.

```csharp
public class RevisionQueryTable : Revision
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CellArea](../../aspose.cells.revisions/revisionquerytable/cellarea/) { get; } | يحصل على موقع جدول الاستعلام المتأثر. |
| [FieldId](../../aspose.cells.revisions/revisionquerytable/fieldid/) { get; } | يحصل على معرف الحقل المحدد في جدول الاستعلام الذي تم إزالته. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | يحصل على رقم هذه المراجعة.(موروث من [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisionquerytable/type/) { get; } | يمثل نوع المراجعة. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | يحصل على ورقة العمل. (موروث من [`Revision`](../revision/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionQueryTableDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // أضف بيانات نموذجية لإنشاء سياق لجدول الاستعلام
                worksheet.Cells["A1"].Value = "Product";
                worksheet.Cells["B1"].Value = "Price";
                worksheet.Cells["A2"].Value = "Apple";
                worksheet.Cells["B2"].Value = 1.20;

                // ملاحظة: عادةً ما يتم الحصول على كائنات RevisionQueryTable من مراجعات المصنف
                // هذا توضيح مفهومي لأننا لا نستطيع إنشاء RevisionQueryTable مباشرةً

                // في سيناريو حقيقي، ستصل إلى المراجعات بهذه الطريقة:
                // RevisionCollection revisions = workbook.Worksheets.Revisions;
                // foreach (Revision revision in revisions)
                // {
                //     if (revision is RevisionQueryTable queryTableRevision)
                //     {
                //         // الوصول إلى الخصائص
                //     }
                // }

                // للتوضيح، سنظهر كيفية العمل مع خصائص RevisionQueryTable
                // إذا كان لدينا نسخة
                Console.WriteLine("RevisionQueryTable properties demonstration:");
                Console.WriteLine("Type property would return: " + RevisionType.QueryTable);
                Console.WriteLine("FieldId property would return an integer ID of the affected field");
                Console.WriteLine("CellArea property would return the location of the query table");

                // احفظ المصنف
                workbook.Save("RevisionQueryTableDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionQueryTable: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


