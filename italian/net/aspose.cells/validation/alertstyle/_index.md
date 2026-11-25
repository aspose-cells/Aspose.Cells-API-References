---
title: "Validation.AlertStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà di convalida. Rappresenta lo stile di avviso della convalida"
type: docs
url: /it/net/aspose.cells/validation/alertstyle/
---
## Validation.AlertStyle property

Rappresenta lo stile di avviso di convalida.

```csharp
public ValidationAlertType AlertStyle { get; set; }
```

### Esempi

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

### Vedi anche

* enum [ValidationAlertType](../../validationalerttype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


