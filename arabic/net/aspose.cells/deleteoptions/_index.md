---
title: "الفئة DeleteOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.DeleteOptions. تمثل إعداد حذف الصفوف/الأعمدة"
type: docs
url: /ar/net/aspose.cells/deleteoptions/
---
## DeleteOptions class

يمثل إعداد حذف الصفوف/الأعمدة.

```csharp
public class DeleteOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [DeleteOptions](deleteoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [FormulaChangeMonitor](../../aspose.cells/deleteoptions/formulachangemonitor/) { get; set; } | يحصل على/يضبط المراقب لتتبع التغييرات الناجمة عن الحذف. |
| [UpdateReference](../../aspose.cells/deleteoptions/updatereference/) { get; set; } | يشير إلى ما إذا كان يتم تحديث المراجع في أوراق العمل الأخرى. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DeleteOptionsDemo
    {
        public static void DeleteOptionsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");

            // عرض البيانات الأصلية
            Console.WriteLine("Original Data:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            // إنشاء DeleteOptions
            DeleteOptions options = new DeleteOptions
            {
                UpdateReference = true // Set to true to update references in other worksheets
            };

            // حذف الصف الثاني (Banana)
            sheet.Cells.DeleteRow(2, options.UpdateReference);

            // عرض البيانات بعد الحذف
            Console.WriteLine("\nData After Deletion:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            // احفظ المصنف
            workbook.Save("DeleteOptionsExample.xlsx");
            workbook.Save("DeleteOptionsExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


