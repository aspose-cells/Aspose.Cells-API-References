---
title: "Cells.UnhideRows"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Desoculta las filas ocultas"
type: docs
url: /es/net/aspose.cells/cells/unhiderows/
---
## Cells.UnhideRows method

Muestra las filas ocultas.

```csharp
public void UnhideRows(int row, int totalRows, double height)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | El índice de fila. |
| totalRows | Int32 | El número de fila. |
| altura | Double | Altura de fila. La altura de la fila se cambiará solo cuando la fila esté oculta y el valor de altura proporcionado sea positivo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnhideRowsWithInt32Int32DoubleDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Ocultar filas 0-4
            cells.HideRows(0, 5);
            
            // Desocultar filas 0-4 con ajuste de altura (-1 para ajuste automático)
            cells.UnhideRows(0, 5, -1);
            
            // Verificar que las filas estén desocultadas
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine($"Row {i} hidden status: {cells.IsRowHidden(i)}");
            }
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


