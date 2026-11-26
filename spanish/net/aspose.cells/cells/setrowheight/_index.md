---
title: "Cells.SetRowHeight"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Establece la altura de la fila especificada"
type: docs
url: /es/net/aspose.cells/cells/setrowheight/
---
## Cells.SetRowHeight method

Establece la altura de la fila especificada.

```csharp
public void SetRowHeight(int row, double height)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila. |
| altura | Double | Altura de la fila. En unidades de punto. Debe estar entre 0 y 409.5. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetRowHeightWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establece la altura de la fila para la primera fila (índice 0) a 25.5 puntos
            cells.SetRowHeight(0, 25.5);

            // Verifica la altura de la fila
            Console.WriteLine("Row height of row 0: " + cells.GetRowHeight(0));
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


