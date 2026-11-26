---
title: "Validation.AlertStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de validación. Representa el estilo de alerta de validación"
type: docs
url: /es/net/aspose.cells/validation/alertstyle/
---
## Validation.AlertStyle property

Representa el estilo de alerta de validación.

```csharp
public ValidationAlertType AlertStyle { get; set; }
```

### Ejemplos

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

### Ver también

* enum [ValidationAlertType](../../validationalerttype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


