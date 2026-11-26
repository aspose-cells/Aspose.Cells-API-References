---
title: "Validation.ErrorMessage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de validación. Representa el mensaje de error de validación de datos"
type: docs
url: /es/net/aspose.cells/validation/errormessage/
---
## Validation.ErrorMessage property

Representa el mensaje de error de validación de datos.

```csharp
public string ErrorMessage { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyErrorMessageDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear validación para la celda A1
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

            // Establecer propiedades del mensaje de error
            validation.ErrorMessage = "Value must be between 10 and 20";
            validation.ErrorTitle = "Invalid Input";
            validation.AlertStyle = ValidationAlertType.Stop;

            // Aplicar la validación y probarla
            worksheet.Cells["A1"].PutValue(5); // Invalid value
            Console.WriteLine("Validation Error Message: " + validation.ErrorMessage);

            // Guarda el libro de trabajo
            workbook.Save("ValidationErrorMessageDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


