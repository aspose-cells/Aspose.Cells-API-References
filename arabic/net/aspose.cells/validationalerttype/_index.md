---
title: "التعداد ValidationAlertType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.ValidationAlertType. يمثل نمط تنبيه التحقق من البيانات"
type: docs
url: /ar/net/aspose.cells/validationalerttype/
---
## ValidationAlertType enumeration

يمثل نمط تنبيه التحقق من البيانات.

```csharp
public enum ValidationAlertType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Information | `0` | نمط تنبيه معلوماتي. |
| Stop | `1` | نمط تنبيه إيقاف. |
| Warning | `2` | نمط تنبيه تحذير. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationAlertTypeDemo
    {
        public static void ValidationAlertTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // حدد نطاق خلايا للتحقق
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);

            // أضف تحققًا إلى ورقة العمل
            ValidationCollection validations = worksheet.Validations;
            int validationIndex = validations.Add(area);
            Validation validation = validations[validationIndex];

            // تعيين خصائص التحقق
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";
            validation.AlertStyle = ValidationAlertType.Stop; // Using the ValidationAlertType enum
            validation.ErrorTitle = "Invalid Input";
            validation.ErrorMessage = "Please enter a number between 3 and 1234.";
            validation.ShowError = true;

            // احفظ المصنف
            workbook.Save("ValidationAlertTypeExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


