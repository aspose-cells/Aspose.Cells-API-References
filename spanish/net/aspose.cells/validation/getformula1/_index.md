---
title: "Validation.GetFormula1"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de validación. Obtiene el valor o expresión asociado con esta validación"
type: docs
url: /es/net/aspose.cells/validation/getformula1/
---
## GetFormula1(bool, bool) {#getformula1}

Obtiene el valor o expresión asociado con esta validación.

```csharp
public string GetFormula1(bool isR1C1, bool isLocal)
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

    public class ValidationMethodGetFormula1WithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añade una validación a la primera celda
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            
            // Aplica la validación a la celda A1
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            try
            {
                // Llama a GetFormula1 con los parámetros (false, false) para obtener la fórmula en notación A1
                string formula1 = validation.GetFormula1(false, false);
                
                Console.WriteLine("Formula1 in A1 notation: " + formula1);
                
                // Llama a GetFormula1 con los parámetros (true, false) para obtener la fórmula en notación R1C1
                string formula1R1C1 = validation.GetFormula1(true, false);
                
                Console.WriteLine("Formula1 in R1C1 notation: " + formula1R1C1);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula1 method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("ValidationMethodGetFormula1WithBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula1(bool, bool, int, int) {#getformula1_1}

Obtiene el valor o expresión asociado con esta validación para una celda específica.

```csharp
public string GetFormula1(bool isR1C1, bool isLocal, int row, int column)
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

    public class ValidationMethodGetFormula1WithBooleanBooleanInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea validación en la celda B5 (fila 4, columna 1)
            CellArea area = CellArea.CreateCellArea(4, 1, 4, 1); // Use static method via type name
            int validationIndex = worksheet.Validations.Add(area); // Get validation index
            Validation validation = worksheet.Validations[validationIndex]; // Retrieve validation object
            validation.Type = ValidationType.Custom;
            validation.Formula1 = "=A5"; // Relative reference to cell A5

            try
            {
                // Llama a GetFormula1 con formato R1C1 para la celda B5
                string formulaR1C1 = validation.GetFormula1(true, false, 4, 1);
                Console.WriteLine($"R1C1 Formula: {formulaR1C1}");

                // Llama a GetFormula1 con formato A1 para la celda B5
                string formulaA1 = validation.GetFormula1(false, false, 4, 1);
                Console.WriteLine($"A1 Formula: {formulaA1}");

                workbook.Save("ValidationGetFormula1Demo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


