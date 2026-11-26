---
title: "Validation.SetFormula1"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de validación. Establece el valor o expresión asociado con esta validación"
type: docs
url: /es/net/aspose.cells/validation/setformula1/
---
## Validation.SetFormula1 method

Establece el valor o expresión asociado con esta validación.

```csharp
public void SetFormula1(string formula, bool isR1C1, bool isLocal)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fórmula | String | El valor o expresión asociado con esta condición de formato. |
| isR1C1 | Booleano | Si la fórmula es una fórmula R1C1. |
| isLocal | Booleano | Si la fórmula está formateada según la configuración regional. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodSetFormula1WithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepare datos de muestra en la celda B1
            worksheet.Cells["B1"].PutValue(100);

            // Crea validación de datos para la celda A1
            int validationIndex = worksheet.Validations.Add(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            Validation validation = worksheet.Validations[validationIndex];
            validation.Type = ValidationType.Decimal;
            validation.Operator = OperatorType.GreaterOrEqual;
            validation.ShowError = true;
            validation.ErrorTitle = "Validation Error";
            validation.ErrorMessage = "Value must be greater than or equal to cell B1 (100)";

            try
            {
                // Establece la fórmula que hace referencia a B1 usando notación A1 (no R1C1, no local)
                validation.SetFormula1("=B1", false, false);
                Console.WriteLine("SetFormula1 executed successfully with parameters (String, Boolean, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula1: {ex.Message}");
            }

            // Guarda el libro de trabajo con la validación
            workbook.Save("ValidationSetFormula1Demo.xlsx");
        }
    }
}
```

### Ver también

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


