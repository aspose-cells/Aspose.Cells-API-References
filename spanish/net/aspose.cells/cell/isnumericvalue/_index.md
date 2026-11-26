---
title: "Cell.IsNumericValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Indica si el valor de esta celda es numérico, entero, doble y datetime"
type: docs
url: /es/net/aspose.cells/cell/isnumericvalue/
---
## Cell.IsNumericValue property

Indica si el valor de esta celda es numérico (int, double y datetime)

```csharp
public bool IsNumericValue { get; }
```

### Observaciones

También se aplica a la celda de fórmula para comprobar el resultado calculado

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsNumericValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar diferentes tipos de datos a las celdas
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue(123.45); // Numeric value

            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Hello World"); // String value

            // Verificar si las celdas contienen valores numéricos
            Console.WriteLine("Cell A1 IsNumericValue: " + cell1.IsNumericValue);
            Console.WriteLine("Cell A2 IsNumericValue: " + cell2.IsNumericValue);

            // Demostrar el uso con lógica condicional
            if (cell1.IsNumericValue)
            {
                Console.WriteLine("Cell A1 contains a numeric value: " + cell1.DoubleValue);
            }

            if (!cell2.IsNumericValue)
            {
                Console.WriteLine("Cell A2 does not contain a numeric value");
            }
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


