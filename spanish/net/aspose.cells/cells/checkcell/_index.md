---
title: "Cells.CheckCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene el elemento Cell o null en el índice de fila y columna de celda especificados"
type: docs
url: /es/net/aspose.cells/cells/checkcell/
---
## Cells.CheckCell method

Obtiene el elemento [`Cell`](../../cell/) o null en el índice de fila y columna de celda especificados.

```csharp
public Cell CheckCell(int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila |
| columna | Int32 | Índice de columna |

### Valor de retorno

Devuelve el objeto Cell si existe un objeto Cell. Devuelve null si la celda no existe.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCheckCellWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer valores en celdas
            cells[0, 0].PutValue("Hello");
            cells[1, 1].PutValue(123);
            cells[2, 2].PutValue(DateTime.Now);

            // Comprobar celdas usando el método CheckCell con parámetros Int32
            Cell cell1 = cells.CheckCell(0, 0);
            Console.WriteLine("Cell A1 value: " + cell1.StringValue);

            Cell cell2 = cells.CheckCell(1, 1);
            Console.WriteLine("Cell B2 value: " + cell2.StringValue);

            Cell cell3 = cells.CheckCell(2, 2);
            Console.WriteLine("Cell C3 value: " + cell3.StringValue);

            // Comprobar celda inexistente (devolverá null)
            Cell cell4 = cells.CheckCell(10, 10);
            if (cell4 == null)
            {
                Console.WriteLine("Cell K11 doesn't exist (as expected)");
            }
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


