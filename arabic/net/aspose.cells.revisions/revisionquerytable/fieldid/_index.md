---
title: "RevisionQueryTable.FieldId"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionQueryTable. تحصل على معرف الحقل المحدد لجدول الاستعلام الذي تم إزالته"
type: docs
url: /ar/net/aspose.cells.revisions/revisionquerytable/fieldid/
---
## RevisionQueryTable.FieldId property

يحصل على معرف الحقل المحدد في جدول الاستعلام الذي تم إزالته.

```csharp
public int FieldId { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionQueryTablePropertyFieldIdDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات النموذجية إلى ورقة العمل
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1.20;

            try
            {
                // إنشاء جدول استعلام (هذا مثال مبسط)
                // ملاحظة: في سيناريو حقيقي، ستحتاج إلى إنشاء جدول استعلام أولاً
                // لأغراض العرض، سنحاكي الوصول إلى RevisionQueryTable

                // نظرًا لأننا لا نستطيع إنشاء RevisionQueryTable مباشرةً في هذا المثال المبسط،
                // سنوضح كيفية الوصول إلى خاصية FieldId إذا كان لدينا واحدة
                // هذا يوضح النمط لقراءة الخاصية للقراءة فقط

                // محاكاة الحصول على RevisionQueryTable من المراجعات (مفهومي)
                // في الواقع، ستحصل على هذا من workbook.Revisions أو ما شابه
                RevisionQueryTable revisionQueryTable = null;

                // تحقق مما إذا كان لدينا جدول استعلام مراجعة (هذا فقط للعرض)
                if (revisionQueryTable != null)
                {
                    // عرض قيمة خاصية FieldId
                    Console.WriteLine("FieldId value: " + revisionQueryTable.FieldId);

                    // عرض خصائص أخرى للسياق
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);
                    Console.WriteLine("Cell Area: " + revisionQueryTable.CellArea);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                }

                // احفظ المصنف
                workbook.Save("FieldIdDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


