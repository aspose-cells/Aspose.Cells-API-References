---
title: "Validation.GetFormula2"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de validación. Obtiene el valor o expresión asociado con esta validación"
type: docs
url: /es/net/aspose.cells/validation/getformula2/
---
## GetFormula2(bool, bool) {#getformula2}

Obtiene el valor o expresión asociado con esta validación.

```csharp
public string GetFormula2(bool isR1C1, bool isLocal)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isR1C1 | Booleano | Si la fórmula necesita formatearse como R1C1. |
| isLocal | Booleano | Si la fórmula necesita formatearse según la configuración regional. |

### Valor de retorno

El valor o expresión asociado con esta validación.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodGetFormula2WithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una validación a un rango de celdas
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            
            // Agregar área de validación
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            try
            {
                // Llamar a GetFormula2 con los parámetros (isR1C1: false, isLocal: false)
                string formula2 = validation.GetFormula2(false, false);
                
                Console.WriteLine("Formula2: " + formula2);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean)");
                
                // Mostrar la configuración de validación
                Console.WriteLine("Validation Type: " + validation.Type);
                Console.WriteLine("Validation Operator: " + validation.Operator);
                Console.WriteLine("Validation Formula1: " + validation.Formula1);
                Console.WriteLine("Validation Formula2: " + validation.Formula2);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula2 method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("ValidationMethodGetFormula2Demo.xlsx");
        }
    }
}
```

### Ver también

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula2(bool, bool, int, int) {#getformula2_1}

Obtiene el valor o expresión asociado con esta validación para una celda específica.

```csharp
public string GetFormula2(bool isR1C1, bool isLocal, int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isR1C1 | Booleano | Si la fórmula necesita formatearse como R1C1. |
| isLocal | Booleano | Si la fórmula necesita formatearse según la configuración regional. |
| fila | Int32 | El índice de fila. |
| columna | Int32 | El índice de columna. |

### Valor de retorno

El valor o expresión asociado con esta validación.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodGetFormula2WithBooleanBooleanInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear validación de datos en la celda A1
            worksheet.Validations.Add();
            Validation validation = worksheet.Validations[worksheet.Validations.Count - 1];
            validation.Type = ValidationType.Custom;
            validation.Operator = OperatorType.Between;
            validation.Formula2 = "=B1"; // A1-style formula
            validation.AddArea(CellArea.CreateCellArea(0, 0, 0, 0)); // Apply to cell A1 (row 0, column 0)

            try
            {
                // Obtener Formula2 en formato R1C1 para la celda A1
                string formulaR1C1 = validation.GetFormula2(true, false, 0, 0);
                Console.WriteLine($"Formula2 (R1C1 format): {formulaR1C1}");

                // Demostrar que la fórmula original permanece sin cambios
                Console.WriteLine($"Original Formula2 (A1 format): {validation.Formula2}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula2: {ex.Message}");
            }

            workbook.Save("ValidationGetFormula2Demo.xlsx");
        }
    }
}
```

### Ver también

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


