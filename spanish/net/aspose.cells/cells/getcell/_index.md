---
title: "Cells.GetCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene el elemento Cell o null en el índice de fila y columna de celda especificados"
type: docs
url: /es/net/aspose.cells/cells/getcell/
---
## Cells.GetCell method

Obtiene el elemento [`Cell`](../../cell/) o null en el índice de fila y columna de celda especificados.

```csharp
[Obsolete("Use Cells.CheckCell(int row, int column) instead.")]
public Cell GetCell(int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila |
| columna | Int32 | Índice de columna |

### Valor de retorno

Devuelve el objeto Cell si existe un objeto Cell. Devuelve null si la celda no existe.

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método CheckCell(int row, int column). Este método será eliminado 12 meses después, a partir de febrero de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetCellWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceder a la celda en la fila 1, columna 2 (índice basado en 0)
            Cell cell = worksheet.Cells.GetCell(1, 2);
            
            // Establecer valor y estilo para demostración
            cell.PutValue("Test Value");
            Style style = cell.GetStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);
            
            // Guarda el libro de trabajo
            workbook.Save("GetCellDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


