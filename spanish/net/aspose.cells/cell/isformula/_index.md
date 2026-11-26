---
title: "Cell.IsFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Representa si la celda especificada contiene una fórmula"
type: docs
url: /es/net/aspose.cells/cell/isformula/
---
## Cell.IsFormula property

Representa si la celda especificada contiene una fórmula.

```csharp
public bool IsFormula { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsFormulaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar fórmula a la celda A1
            worksheet.Cells["A1"].Formula = "=1+2";
            
            // Agregar valor simple a la celda A2
            worksheet.Cells["A2"].PutValue("Test");
            
            // Verificar si las celdas contienen fórmulas
            Console.WriteLine("A1 is formula: " + worksheet.Cells["A1"].IsFormula);
            Console.WriteLine("A2 is formula: " + worksheet.Cells["A2"].IsFormula);
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


