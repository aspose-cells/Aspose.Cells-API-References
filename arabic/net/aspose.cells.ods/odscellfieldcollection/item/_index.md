---
title: "OdsCellFieldCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OdsCellFieldCollection. تحصل على الحقل حسب الفهرس"
type: docs
url: /ar/net/aspose.cells.ods/odscellfieldcollection/item/
---
## OdsCellFieldCollection indexer (1 of 2)

تحصل على الحقل حسب الفهرس.

```csharp
public OdsCellField this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة حقول خلايا ODS بمعامل التنسيق
            sheet.Cells.OdsCellFields.Add(0, 0, OdsCellFieldType.Title, "");
            sheet.Cells.OdsCellFields.Add(0, 1, OdsCellFieldType.SheetName, "");

            // الوصول إلى الحقول باستخدام خاصية Item
            OdsCellField titleField = sheet.Cells.OdsCellFields[0];
            OdsCellField sheetNameField = sheet.Cells.OdsCellFields[1];

            // إخراج أنواع الحقول
            Console.WriteLine("Field 0 Type: " + titleField.FieldType);
            Console.WriteLine("Field 1 Type: " + sheetNameField.FieldType);

            // حفظ وإعادة تحميل
            workbook.Save("output.ods");
            workbook = new Workbook("output.ods");
            sheet = workbook.Worksheets[0];

            // التحقق من الحقول المحفوظة
            Console.WriteLine("Reloaded Field 0 Type: " + sheet.Cells.OdsCellFields[0].FieldType);
            Console.WriteLine("Reloaded Field 1 Type: " + sheet.Cells.OdsCellFields[1].FieldType);
        }
    }
}
```

### انظر أيضًا

* class [OdsCellField](../../odscellfield/)
* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)

---

## OdsCellFieldCollection indexer (2 of 2)

تحصل على الحقل حسب فهرس الصف والعمود.

```csharp
public OdsCellField this[int row, int column] { get; }
```

| معامل | الوصف |
| --- | --- |
| صف | فهرس الصف. |
| عمود | فهرس العمود. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بعض حقول خلايا ODS
            // (صف, عمود, نوع الحقل, تنسيق)
            sheet.Cells.OdsCellFields.Add(0, 0, OdsCellFieldType.Title, "TitleFormat");
            sheet.Cells.OdsCellFields.Add(1, 1, OdsCellFieldType.SheetName, null);

            try
            {
                // الوصول إلى الحقول باستخدام خاصية Item (المؤشر)
                // 1) حسب فهرس المجموعة
                OdsCellField firstField = sheet.Cells.OdsCellFields[0];
                Console.WriteLine("First field type (by index): " + firstField.FieldType);

                // 2) حسب موضع الخلية (صف، عمود)
                OdsCellField titleField = sheet.Cells.OdsCellFields[0, 0];
                Console.WriteLine("Field at (0,0) type (by position): " + titleField.FieldType);

                // تحديث الخلايا بقيم الحقول
                sheet.Cells.OdsCellFields.UpdateFieldsValue();

                // حفظ المصنف (صيغة ODS تحافظ على الحقول)
                workbook.Save("OdsCellFieldItemDemo.ods");
                Console.WriteLine("Workbook saved as OdsCellFieldItemDemo.ods");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### انظر أيضًا

* class [OdsCellField](../../odscellfield/)
* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


