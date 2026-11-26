---
title: "Cell.IsSharedFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Indica si la fórmula de la celda forma parte de una fórmula compartida"
type: docs
url: /es/net/aspose.cells/cell/issharedformula/
---
## Cell.IsSharedFormula property

Indica si la fórmula de la celda forma parte de una fórmula compartida.

```csharp
public bool IsSharedFormula { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsSharedFormulaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer fórmula compartida en un rango
            worksheet.Cells["B2"].Formula = "=A2*2";
            worksheet.Cells["B2"].Copy(worksheet.Cells["B3:B5"]);

            // Verificar si las celdas contienen fórmula compartida
            Cell cellB2 = worksheet.Cells["B2"];
            Cell cellB3 = worksheet.Cells["B3"];

            Console.WriteLine("Cell B2 IsSharedFormula: " + cellB2.IsSharedFormula);
            Console.WriteLine("Cell B3 IsSharedFormula: " + cellB3.IsSharedFormula);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


