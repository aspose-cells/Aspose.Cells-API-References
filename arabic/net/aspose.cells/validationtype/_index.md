---
title: "تعداد ValidationType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.ValidationType تعداد. يمثل نوع التحقق من البيانات"
type: docs
url: /ar/net/aspose.cells/validationtype/
---
## ValidationType enumeration

يمثل نوع التحقق من البيانات.

```csharp
public enum ValidationType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| AnyValue | `0` | نوع تحقق أي قيمة. |
| WholeNumber | `1` | نوع تحقق عدد صحيح. |
| Decimal | `2` | نوع تحقق عدد عشري. |
| List | `3` | نوع تحقق قائمة. |
| Date | `4` | نوع تحقق تاريخ. |
| Time | `5` | نوع تحقق وقت. |
| TextLength | `6` | نوع تحقق طول النص. |
| Custom | `7` | نوع تحقق مخصص. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationTypeDemo
    {
        public static void ValidationTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف تحققًا إلى ورقة العمل
            ValidationCollection validations = worksheet.Validations;
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
            Validation validation = validations[validations.Add(area)];

            // تعيين نوع التحقق إلى WholeNumber
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";

            // تعيين خصائص إضافية للتحقق
            validation.InputMessage = "Please enter a whole number between 3 and 1234.";
            validation.InputTitle = "Whole Number Validation";
            validation.ErrorMessage = "The value must be a whole number between 3 and 1234.";
            validation.ErrorTitle = "Invalid Input";
            validation.ShowInput = true;
            validation.ShowError = true;

            // احفظ المصنف
            workbook.Save("ValidationTypeExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


