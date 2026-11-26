---
title: "Enumeración ValidationType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.ValidationType. Representa el tipo de validación de datos"
type: docs
url: /es/net/aspose.cells/validationtype/
---
## ValidationType enumeration

Representa el tipo de validación de datos.

```csharp
public enum ValidationType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| AnyValue | `0` | Tipo de validación de cualquier valor. |
| WholeNumber | `1` | Tipo de validación de número entero. |
| Decimal | `2` | Tipo de validación decimal. |
| List | `3` | Tipo de validación de lista. |
| Date | `4` | Tipo de validación de fecha. |
| Time | `5` | Tipo de validación de hora. |
| TextLength | `6` | Tipo de validación de longitud de texto. |
| Custom | `7` | Tipo de validación personalizada. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationTypeDemo
    {
        public static void ValidationTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una validación a la hoja de cálculo
            ValidationCollection validations = worksheet.Validations;
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
            Validation validation = validations[validations.Add(area)];

            // Establecer el tipo de validación a WholeNumber
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";

            // Establecer propiedades adicionales para la validación
            validation.InputMessage = "Please enter a whole number between 3 and 1234.";
            validation.InputTitle = "Whole Number Validation";
            validation.ErrorMessage = "The value must be a whole number between 3 and 1234.";
            validation.ErrorTitle = "Invalid Input";
            validation.ShowInput = true;
            validation.ShowError = true;

            // Guarda el libro de trabajo
            workbook.Save("ValidationTypeExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


