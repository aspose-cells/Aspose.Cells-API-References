---
title: "Validation.ErrorMessage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Validation. تمثل رسالة خطأ التحقق من البيانات"
type: docs
url: /ar/net/aspose.cells/validation/errormessage/
---
## Validation.ErrorMessage property

يمثل رسالة خطأ التحقق من البيانات.

```csharp
public string ErrorMessage { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyErrorMessageDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء التحقق للخلية A1
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            Validation validation = worksheet.Validations[worksheet.Validations.Add(area)];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";

            // تعيين خصائص رسالة الخطأ
            validation.ErrorMessage = "Value must be between 10 and 20";
            validation.ErrorTitle = "Invalid Input";
            validation.AlertStyle = ValidationAlertType.Stop;

            // تطبيق التحقق واختباره
            worksheet.Cells["A1"].PutValue(5); // Invalid value
            Console.WriteLine("Validation Error Message: " + validation.ErrorMessage);

            // احفظ المصنف
            workbook.Save("ValidationErrorMessageDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


