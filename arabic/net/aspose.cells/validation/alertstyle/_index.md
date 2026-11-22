---
title: "Validation.AlertStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Validation. تمثل نمط تنبيه التحقق"
type: docs
url: /ar/net/aspose.cells/validation/alertstyle/
---
## Validation.AlertStyle property

يمثل نمط تنبيه التحقق.

```csharp
public ValidationAlertType AlertStyle { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyAlertStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.AddArea(CellArea.CreateCellArea(0, 0, 1, 1));
            
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";
            validation.AlertStyle = ValidationAlertType.Stop;
            validation.ErrorTitle = "Invalid Input";
            validation.ErrorMessage = "Please enter a number between 3 and 1234";
            validation.ShowError = true;

            workbook.Save("ValidationAlertStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ValidationAlertType](../../validationalerttype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


