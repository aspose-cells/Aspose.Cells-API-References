---
title: "RevisionQueryTable.CellArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionQueryTable. تحصل على موقع جدول الاستعلام المتأثر"
type: docs
url: /ar/net/aspose.cells.revisions/revisionquerytable/cellarea/
---
## RevisionQueryTable.CellArea property

يحصل على موقع جدول الاستعلام المتأثر.

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

    public class RevisionQueryTablePropertyCellAreaDemo
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
                RevisionQueryTable revisionQueryTable = null;

                // تحقق مما إذا كان لدينا جدول استعلام مراجعة
                if (revisionQueryTable != null)
                {
                    // عرض قيمة خاصية CellArea (للقراءة فقط)
                    Console.WriteLine("CellArea value: " + revisionQueryTable.CellArea);

                    // عرض خصائص أخرى للسياق
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);
                    Console.WriteLine("Field ID: " + revisionQueryTable.FieldId);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                    Console.WriteLine("Sample CellArea demonstration:");
                    Console.WriteLine("CellArea would represent the location of the query table, e.g., 'A1:B2'");
                }

                // احفظ المصنف
                workbook.Save("CellAreaDemo.xlsx");
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

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


