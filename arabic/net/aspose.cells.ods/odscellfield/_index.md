---
title: "الفئة OdsCellField"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Ods.OdsCellField. تمثل حقل الخلية في ods"
type: docs
url: /ar/net/aspose.cells.ods/odscellfield/
---
## OdsCellField class

يمثل حقل الخلية في ods.

```csharp
public class OdsCellField
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Column](../../aspose.cells.ods/odscellfield/column/) { get; set; } | يحصل على ويضبط فهرس العمود للخلية. |
| [CustomFormat](../../aspose.cells.ods/odscellfield/customformat/) { get; set; } | يمثل التنسيق المخصص لقيمة الحقل. |
| [FieldType](../../aspose.cells.ods/odscellfield/fieldtype/) { get; set; } | يحصل على ويضبط نوع الحقل. |
| [Row](../../aspose.cells.ods/odscellfield/row/) { get; set; } | يحصل على ويضبط فهرس الصف للخلية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Ods;

    public class OdsClassOdsCellFieldDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            try
            {
                // -----------------------------------------------------------------
                // 1. إنشاء OdsCellField عبر المجموعة (بدون مُنشئ بدون معلمات)
                // -----------------------------------------------------------------
                OdsCellFieldCollection odsFields = sheet.Cells.OdsCellFields;
                odsFields.Add(2, 1, OdsCellFieldType.Title, "Demo Title");

                // استرجاع الحقل الذي أضفناه للتو
                OdsCellField manualField = odsFields[odsFields.Count - 1];

                // اكتب شيئًا إلى الخلية المحددة بواسطة OdsCellField
                sheet.Cells[manualField.Row, manualField.Column].PutValue("Manual Field");

                // --------------------------------------------------------------
                // 2. إضافة نفس الحقل مرة أخرى لتوضيح استخدام المجموعة (اختياري)
                // --------------------------------------------------------------
                odsFields.Add(manualField.Row, manualField.Column, manualField.FieldType, manualField.CustomFormat);

                // تحديث جميع حقول ODS بحيث تنعكس في الملف المحفوظ
                odsFields.UpdateFieldsValue();

                // عرض قيم الخصائص في وحدة التحكم
                Console.WriteLine($"Created OdsCellField -> Row: {manualField.Row}, Column: {manualField.Column}, " +
                                  $"Type: {manualField.FieldType}, Format: {manualField.CustomFormat}");

                // حفظ المصنف كملف ODS
                workbook.Save("OdsClassOdsCellFieldDemo.ods");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while working with OdsCellField: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


