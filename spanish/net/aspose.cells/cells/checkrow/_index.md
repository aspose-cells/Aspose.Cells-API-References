---
title: "Cells.CheckRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene el elemento Row o null en el índice de fila de celda especificado"
type: docs
url: /es/net/aspose.cells/cells/checkrow/
---
## Cells.CheckRow method

Obtiene el elemento [`Row`](../../row/) o null en el índice de fila de celda especificado.

```csharp
public Row CheckRow(int row)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila |

### Valor de retorno

Devuelve el objeto [`Row`](../../row/) si el objeto fila existe, de lo contrario devuelve null.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCheckRowWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Poblar algunos datos
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue(100);
            cells["A3"].PutValue(200);
            
            // Verificar si la fila existe y obtener el objeto fila
            Row row = cells.CheckRow(1);
            if (row != null)
            {
                Console.WriteLine("Row 1 exists with height: " + row.Height);
            }
            
            // Verificar fila inexistente
            Row nonExistentRow = cells.CheckRow(100);
            Console.WriteLine("Row 100 exists: " + (nonExistentRow != null));
        }
    }
}
```

### Ver también

* class [Row](../../row/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


