---
title: "Cells.UnhideColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Desoculta una columna"
type: docs
url: /es/net/aspose.cells/cells/unhidecolumn/
---
## Cells.UnhideColumn method

Muestra una columna

```csharp
public void UnhideColumn(int column, double width)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | Int32 | Índice de columna. |
| ancho | Double | Ancho de columna. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnhideColumnWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Ocultar columna 2
            cells.HideColumn(2);
            
            // Mostrar columna 2 con ajuste de ancho (-1 significa usar el ancho estándar)
            cells.UnhideColumn(2, -1);
            
            Console.WriteLine("Column 2 width after unhiding: " + cells.Columns[2].Width);
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


