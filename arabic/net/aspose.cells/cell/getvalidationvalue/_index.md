---
title: "Cell.GetValidationValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. تحصل على قيمة التحقق التي تم تطبيقها على هذه الخلية"
type: docs
url: /ar/net/aspose.cells/cell/getvalidationvalue/
---
## Cell.GetValidationValue method

يحصل على قيمة التحقق التي تم تطبيقها على هذه الخلية.

```csharp
public bool GetValidationValue()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetValidationValueDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نطاق تحقق
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.TextLength;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "1";
            validation.Formula2 = "5";

            // تطبيق التحقق على الخلية A1
            Cell cell = worksheet.Cells["A1"];
            validation.AddArea(new CellArea { StartRow = cell.Row, StartColumn = cell.Column, EndRow = cell.Row, EndColumn = cell.Column });

            // اختبار القيم الصالحة
            string[] validValues = { "a", " ab", "cd ", " xyz " };
            foreach (string value in validValues)
            {
                cell.PutValue(value);
                Console.WriteLine($"Value: '{value}' - Valid: {cell.GetValidationValue()}");
            }

            // اختبار قيمة غير صالحة
            string invalidValue = "toolong";
            cell.PutValue(invalidValue);
            Console.WriteLine($"Value: '{invalidValue}' - Valid: {cell.GetValidationValue()}");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


