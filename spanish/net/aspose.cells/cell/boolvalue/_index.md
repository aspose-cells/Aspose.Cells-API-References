---
title: "Cell.BoolValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Cell. Obtiene el valor booleano contenido en la celda"
type: docs
url: /es/net/aspose.cells/cell/boolvalue/
---
## Cell.BoolValue property

Obtiene el valor booleano contenido en la celda.

```csharp
public bool BoolValue { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyBoolValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Cell cell = cells[0, 0];
            
            // Establecer una fórmula que evalúe a un valor booleano
            cell.Formula = "=2.01>2";
            
            // Calcular la fórmula para obtener el resultado
            workbook.CalculateFormula();
            
            // Demostrar la propiedad BoolValue
            Console.WriteLine("Cell BoolValue: " + cell.BoolValue);
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


