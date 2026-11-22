---
title: "Cells.OdsCellFields"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. تحصل على قائمة الحقول في ods"
type: docs
url: /ar/net/aspose.cells/cells/odscellfields/
---
## Cells.OdsCellFields property

يحصل على قائمة الحقول في ods.

```csharp
public OdsCellFieldCollection OdsCellFields { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsPropertyOdsCellFieldsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // احصل على مجموعة Cells
            Cells cells = worksheet.Cells;

            try
            {
                // الوصول إلى خاصية OdsCellFields (للقراءة فقط)
                var odsCellFields = cells.OdsCellFields;

                // عرض معلومات حول مجموعة OdsCellFields
                Console.WriteLine("OdsCellFields collection count: " + odsCellFields.Count);

                // التكرار عبر مجموعة OdsCellFields
                for (int i = 0; i < odsCellFields.Count; i++)
                {
                    var field = odsCellFields[i];
                    Console.WriteLine($"Field {i}: Type - {field.FieldType}");
                }

                // إظهار تحديث قيم الحقول
                odsCellFields.UpdateFieldsValue();

                Console.WriteLine("OdsCellFields demonstration completed successfully.");
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

* class [OdsCellFieldCollection](../../../aspose.cells.ods/odscellfieldcollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


