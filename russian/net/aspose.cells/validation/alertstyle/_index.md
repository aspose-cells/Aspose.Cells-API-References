---
title: "Validation.AlertStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Validation. Представляет стиль оповещения проверки"
type: docs
url: /ru/net/aspose.cells/validation/alertstyle/
---
## Validation.AlertStyle property

Представляет стиль оповещения проверки.

```csharp
public ValidationAlertType AlertStyle { get; set; }
```

### Примеры

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

### См. также

* enum [ValidationAlertType](../../validationalerttype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


