---
title: "Cell.GetValidationValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Obtiene el valor de validación que se aplica a esta celda"
type: docs
url: /es/net/aspose.cells/cell/getvalidationvalue/
---
## Cell.GetValidationValue method

Obtiene el valor de validación que se aplica a esta celda.

```csharp
public bool GetValidationValue()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetValidationValueDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un rango de validación
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.TextLength;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "1";
            validation.Formula2 = "5";

            // Aplica la validación a la celda A1
            Cell cell = worksheet.Cells["A1"];
            validation.AddArea(new CellArea { StartRow = cell.Row, StartColumn = cell.Column, EndRow = cell.Row, EndColumn = cell.Column });

            // Probar valores válidos
            string[] validValues = { "a", " ab", "cd ", " xyz " };
            foreach (string value in validValues)
            {
                cell.PutValue(value);
                Console.WriteLine($"Value: '{value}' - Valid: {cell.GetValidationValue()}");
            }

            // Probar valor inválido
            string invalidValue = "toolong";
            cell.PutValue(invalidValue);
            Console.WriteLine($"Value: '{invalidValue}' - Valid: {cell.GetValidationValue()}");
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


