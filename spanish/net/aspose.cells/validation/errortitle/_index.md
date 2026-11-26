---
title: "Validation.ErrorTitle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de validación. Representa el título del cuadro de diálogo de error de validación de datos"
type: docs
url: /es/net/aspose.cells/validation/errortitle/
---
## Validation.ErrorTitle property

Representa el título del cuadro de diálogo de error de validación de datos.

```csharp
public string ErrorTitle { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyErrorTitleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Validation validation = worksheet.Validations[worksheet.Validations.Add(CellArea.CreateCellArea(0, 0, 1, 1))];
            
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";
            
            validation.ErrorTitle = "Invalid Input";
            validation.ErrorMessage = "Value must be between 3 and 1234";
            validation.ShowError = true;

            workbook.Save("ValidationErrorTitleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


