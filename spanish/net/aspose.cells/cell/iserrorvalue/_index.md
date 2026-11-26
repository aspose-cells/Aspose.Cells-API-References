---
title: "Cell.IsErrorValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Verifica si el valor de esta celda es un error"
type: docs
url: /es/net/aspose.cells/cell/iserrorvalue/
---
## Cell.IsErrorValue property

Comprueba si el valor de esta celda es un error.

```csharp
public bool IsErrorValue { get; }
```

### Observaciones

También se aplica a la celda de fórmula para comprobar si el resultado calculado es un error.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsErrorValueDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer una fórmula que resulte en un error
            Cell cell = cells["A1"];
            cell.Formula = "=1/0"; // Division by zero error
            
            // Calcular fórmulas
            workbook.CalculateFormula();

            // Demostrar la propiedad IsErrorValue
            Console.WriteLine("Cell A1 value: " + cell.StringValue);
            Console.WriteLine("IsErrorValue: " + cell.IsErrorValue);
            Console.WriteLine("Error type: " + cell.Value);

            // Establecer un valor válido
            Cell cell2 = cells["A2"];
            cell2.PutValue("Valid value");
            
            Console.WriteLine("\nCell A2 value: " + cell2.StringValue);
            Console.WriteLine("IsErrorValue: " + cell2.IsErrorValue);

            // Establecer un error SPILL (error de fórmula de matriz dinámica de Excel 365+)
            Cell cell3 = cells["A3"];
            cell3.SetDynamicArrayFormula("=A1:A10", new FormulaParseOptions(), true);
            
            Console.WriteLine("\nCell A3 value: " + cell3.StringValue);
            Console.WriteLine("IsErrorValue: " + cell3.IsErrorValue);
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


