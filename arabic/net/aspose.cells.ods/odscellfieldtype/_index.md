---
title: "Enum OdsCellFieldType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Ods.OdsCellFieldType enum. يمثل نوع حقل الخلية في ods"
type: docs
url: /ar/net/aspose.cells.ods/odscellfieldtype/
---
## OdsCellFieldType enumeration

يمثل نوع حقل الخلية في ods.

```csharp
public enum OdsCellFieldType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Date | `0` | التاريخ الحالي. |
| SheetName | `1` | اسم الورقة. |
| Title | `2` | اسم الملف. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OdsCellFieldTypeDemo
    {
        public static void OdsCellFieldTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء OdsCellFieldCollection
            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;

            // إضافة OdsCellField جديد للتاريخ الحالي
            int rowIndex = 0;
            int columnIndex = 0;
            string customFormat = "yyyy-mm-dd";
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.Date, customFormat);

            // إضافة OdsCellField آخر لاسم الورقة
            rowIndex = 1;
            columnIndex = 0;
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.SheetName, null);

            // إضافة OdsCellField آخر للعنوان
            rowIndex = 2;
            columnIndex = 0;
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.Title, null);

            // تحديث قيمة الحقول إلى الخلايا
            odsCellFields.UpdateFieldsValue();

            // إخراج القيم في وحدة التحكم
            for (int i = 0; i < odsCellFields.Count; i++)
            {
                OdsCellField field = odsCellFields[i];
                worksheet.Cells[field.Row, field.Column].PutValue($"Field Type: {field.FieldType}, Custom Format: {field.CustomFormat}");
            }

            // احفظ المصنف
            workbook.Save("OdsCellFieldTypeExample.ods");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


