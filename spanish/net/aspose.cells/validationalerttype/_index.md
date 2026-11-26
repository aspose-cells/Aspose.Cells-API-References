---
title: "Enumeración ValidationAlertType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.ValidationAlertType. Representa el estilo de alerta de validación de datos"
type: docs
url: /es/net/aspose.cells/validationalerttype/
---
## ValidationAlertType enumeration

Representa el estilo de alerta de validación de datos.

```csharp
public enum ValidationAlertType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Information | `0` | Estilo de alerta de información. |
| Stop | `1` | Estilo de alerta de detención. |
| Warning | `2` | Estilo de alerta de advertencia. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationAlertTypeDemo
    {
        public static void ValidationAlertTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Definir un área de celdas para la validación
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);

            // Agregar una validación a la hoja de cálculo
            ValidationCollection validations = worksheet.Validations;
            int validationIndex = validations.Add(area);
            Validation validation = validations[validationIndex];

            // Establezca propiedades de validación
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";
            validation.AlertStyle = ValidationAlertType.Stop; // Using the ValidationAlertType enum
            validation.ErrorTitle = "Invalid Input";
            validation.ErrorMessage = "Please enter a number between 3 and 1234.";
            validation.ShowError = true;

            // Guarda el libro de trabajo
            workbook.Save("ValidationAlertTypeExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


