---
title: "Cells.GetRowHeightPixel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene la altura de una fila especificada en unidades de píxel"
type: docs
url: /es/net/aspose.cells/cells/getrowheightpixel/
---
## Cells.GetRowHeightPixel method

Obtiene la altura de una fila especificada en unidades de píxel.

```csharp
public int GetRowHeightPixel(int row)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila |

### Valor de retorno

Altura de la fila

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetRowHeightPixelWithInt32Demo
    {
        public static void Run()
        {
            // Instanciar un nuevo Workbook
            Workbook wb = new Workbook();

            // Obtener la primera hoja de cálculo
            Worksheet worksheet = wb.Worksheets[0];

            // Establecer la altura de la fila 5 (en píxeles)
            worksheet.Cells.SetRowHeightPixel(5, 30);

            // Obtener la altura de la fila 5 (en píxeles)
            int rowHeight = worksheet.Cells.GetRowHeightPixel(5);

            Console.WriteLine("Row height of row 5 in pixels: " + rowHeight);
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


