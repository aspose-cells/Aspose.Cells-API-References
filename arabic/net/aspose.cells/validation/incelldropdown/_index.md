---
title: "Validation.InCellDropDown"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Validation. تشير إلى ما إذا كان التحقق من البيانات يعرض قائمة منسدلة تحتوي على القيم المقبولة"
type: docs
url: /ar/net/aspose.cells/validation/incelldropdown/
---
## Validation.InCellDropDown property

يشير إلى ما إذا كان التحقق من البيانات يعرض قائمة منسدلة تحتوي على القيم المقبولة.

```csharp
public bool InCellDropDown { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyInCellDropDownDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء تحقق للخلية A1
            Validation validation = worksheet.Cells["A1"].GetValidation();
            
            // تعيين نوع التحقق إلى قائمة بالقيم
            validation.Type = ValidationType.List;
            validation.Formula1 = "Option1,Option2,Option3";
            
            // تمكين القائمة المنسدلة داخل الخلية
            validation.InCellDropDown = true;

            // إنشاء تحقق آخر للخلية B1 بدون قائمة منسدلة
            Validation validation2 = worksheet.Cells["B1"].GetValidation();
            validation2.Type = ValidationType.List;
            validation2.Formula1 = "Choice1,Choice2,Choice3";
            validation2.InCellDropDown = false;

            // احفظ المصنف
            workbook.Save("InCellDropDownDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


