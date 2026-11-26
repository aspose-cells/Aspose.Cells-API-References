---
title: "Cell.IsArrayFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Indica si la fórmula de la celda es una fórmula de matriz"
type: docs
url: /es/net/aspose.cells/cell/isarrayformula/
---
## Cell.IsArrayFormula property

Indica si la fórmula de la celda es una fórmula de matriz.

```csharp
public bool IsArrayFormula { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsArrayFormulaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear una fórmula de matriz en la celda B2
            worksheet.Cells["B2"].SetArrayFormula("SUM(A1:A10*B1:B10)", 1, 1);
            
            // Verificar si la celda contiene una fórmula de matriz
            bool isArrayFormula = worksheet.Cells["B2"].IsArrayFormula;
            
            // Mostrar el resultado
            Console.WriteLine("Cell B2 is an array formula: " + isArrayFormula);
            
            // Guarda el libro de trabajo
            workbook.Save("IsArrayFormulaDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


