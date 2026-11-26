---
title: "Cell.IntValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Obtiene el valor entero contenido en la celda"
type: docs
url: /es/net/aspose.cells/cell/intvalue/
---
## Cell.IntValue property

Obtiene el valor entero contenido en la celda.

```csharp
public int IntValue { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIntValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Establece un valor numérico y obtén IntValue
            Cell cell1 = cells[0, 0];
            cell1.PutValue(42);
            Console.WriteLine("IntValue of numeric cell: " + cell1.IntValue);

            // Establece una fórmula que evalúa a un número y obtén IntValue
            Cell cell2 = cells[0, 1];
            cell2.Formula = "=10+5";
            workbook.CalculateFormula();
            Console.WriteLine("IntValue of formula cell: " + cell2.IntValue);

            // Establece un valor booleano y obtén IntValue
            Cell cell3 = cells[0, 2];
            cell3.PutValue(true);
            Console.WriteLine("IntValue of boolean cell: " + cell3.IntValue);

            // Establece un valor de texto y obtén IntValue (será 0 si no es convertible)
            Cell cell4 = cells[0, 3];
            cell4.PutValue("Hello");
            Console.WriteLine("IntValue of text cell: " + cell4.IntValue);
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


