---
title: "Validation.ShowError"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Validation. Indica si el mensaje de error de validación de datos se mostrará siempre que el usuario introduzca datos no válidos"
type: docs
url: /es/net/aspose.cells/validation/showerror/
---
## Validation.ShowError property

Indica si el mensaje de error de validación de datos se mostrará siempre que el usuario ingrese datos no válidos.

```csharp
public bool ShowError { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyShowErrorDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear validación para la celda A1
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            
            // Establezca propiedades de validación
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            
            // Configura la alerta de error
            validation.ShowError = true;
            validation.ErrorTitle = "Invalid Input";
            validation.ErrorMessage = "Value must be between 10 and 20";

            // Crea otra validación para demostrar la copia de propiedades
            Validation targetValidation = worksheet.Validations[worksheet.Validations.Add()];
            targetValidation.AddArea(new CellArea { StartRow = 1, StartColumn = 0, EndRow = 1, EndColumn = 0 });

            // Copia ShowError y las propiedades relacionadas de la primera validación
            targetValidation.ShowError = validation.ShowError;
            targetValidation.ErrorTitle = validation.ErrorTitle;
            targetValidation.ErrorMessage = validation.ErrorMessage;

            // Guarda el libro de trabajo
            workbook.Save("ValidationShowErrorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


