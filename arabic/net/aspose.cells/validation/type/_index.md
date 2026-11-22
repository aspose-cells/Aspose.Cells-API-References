---
title: "Validation.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Validation. تمثل نوع التحقق من البيانات"
type: docs
url: /ar/net/aspose.cells/validation/type/
---
## Validation.Type property

يمثل نوع التحقق من البيانات.

```csharp
public ValidationType Type { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تحقق إلى الخلية A1
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.ErrorTitle = "Number Validation";
            validation.ErrorMessage = "Please enter a whole number";
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });

            // عرض خاصية Type
            Console.WriteLine("Validation Type: " + validation.Type);
            
            // احفظ المصنف
            workbook.Save("ValidationExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ValidationType](../../validationtype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


