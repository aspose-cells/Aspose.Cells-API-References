---
title: "RevisionQueryTable.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionQueryTable. تمثل نوع المراجعة"
type: docs
url: /ar/net/aspose.cells.revisions/revisionquerytable/type/
---
## RevisionQueryTable.Type property

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

    public class RevisionQueryTablePropertyTypeDemo
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
                // في سيناريو حقيقي، ستحصل على المراجعات من workbook
                // للعرض، سننشئ مثالًا مفهوميًا
                // ملاحظة: عادةً ما يتم الحصول على كائنات RevisionQueryTable من مراجعات المصنف

                // إنشاء RevisionQueryTable تجريبي (هذا مفهوم - في الواقع ستحصل عليه من المراجعات)
                // نظرًا لأننا لا نستطيع إنشاء كائن RevisionQueryTable مباشرةً، سنوضح النمط
                RevisionQueryTable revisionQueryTable = null;

                // تحقق مما إذا كان لدينا جدول استعلام مراجعة
                if (revisionQueryTable != null)
                {
                    // عرض قيمة خاصية Type (للقراءة فقط)
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);

                    // إظهار قيمة التعداد كعدد صحيح للمرجع
                    Console.WriteLine("Revision Type (numeric): " + (int)revisionQueryTable.Type);

                    // عرض خصائص أخرى للسياق
                    Console.WriteLine("Cell Area: " + revisionQueryTable.CellArea);
                    Console.WriteLine("Field ID: " + revisionQueryTable.FieldId);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                    Console.WriteLine("Sample RevisionType values:");
                    Console.WriteLine("QueryTable = " + (int)RevisionType.QueryTable);
                    Console.WriteLine("ChangeCells = " + (int)RevisionType.ChangeCells);
                    Console.WriteLine("InsertSheet = " + (int)RevisionType.InsertSheet);
                }

                // احفظ المصنف
                workbook.Save("TypeDemo.xlsx");
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


