---
title: "Validation.ShowError"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Validation. تشير إلى ما إذا كانت رسالة خطأ التحقق من البيانات ستُعرض كلما أدخل المستخدم بيانات غير صالحة"
type: docs
url: /ar/net/aspose.cells/validation/showerror/
---
## Validation.ShowError property

يشير إلى ما إذا كانت رسالة خطأ التحقق من البيانات ستُعرض كلما أدخل المستخدم بيانات غير صالحة.

```csharp
public bool ShowError { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyShowErrorDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء التحقق للخلية A1
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            
            // تعيين خصائص التحقق
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            
            // تكوين تنبيه الخطأ
            validation.ShowError = true;
            validation.ErrorTitle = "Invalid Input";
            validation.ErrorMessage = "Value must be between 10 and 20";

            // إنشاء تحقق آخر لتوضيح نسخ الخاصية
            Validation targetValidation = worksheet.Validations[worksheet.Validations.Add()];
            targetValidation.AddArea(new CellArea { StartRow = 1, StartColumn = 0, EndRow = 1, EndColumn = 0 });

            // نسخ ShowError والخصائص المرتبطة من التحقق الأول
            targetValidation.ShowError = validation.ShowError;
            targetValidation.ErrorTitle = validation.ErrorTitle;
            targetValidation.ErrorMessage = validation.ErrorMessage;

            // احفظ المصنف
            workbook.Save("ValidationShowErrorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


