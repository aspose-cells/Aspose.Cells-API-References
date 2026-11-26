---
title: "Cell.IsArrayHeader"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Indica que la fórmula de la celda es una fórmula de matriz y que es la primera celda de la matriz"
type: docs
url: /es/net/aspose.cells/cell/isarrayheader/
---
## Cell.IsArrayHeader property

Indica que la fórmula de la celda es una fórmula de matriz y que es la primera celda de la matriz.

```csharp
public bool IsArrayHeader { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsArrayHeaderDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea una fórmula de matriz en el rango B2:D4
            worksheet.Cells["B2"].SetArrayFormula("=A1:A3*B1:B3", 3, 3);
            
            // Verifica e imprime la propiedad IsArrayHeader
            // Nota: IsArrayHeader es de solo lectura y se establece automáticamente para los encabezados de fórmulas de matriz
            Console.WriteLine("B2 IsArrayHeader: " + worksheet.Cells["B2"].IsArrayHeader);
            Console.WriteLine("B3 IsArrayHeader: " + worksheet.Cells["B3"].IsArrayHeader);
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


