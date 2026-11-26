---
title: "Cells.CheckColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene el elemento Column o null en el índice de columna especificado"
type: docs
url: /es/net/aspose.cells/cells/checkcolumn/
---
## Cells.CheckColumn method

Obtiene el elemento [`Column`](../../column/) o null en el índice de columna especificado.

```csharp
public Column CheckColumn(int columnIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | Int32 | El índice de columna. |

### Valor de retorno

El objeto Column.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCheckColumnWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Establecer un valor en la columna 1 (B3)
            cells["B3"].PutValue("Sample Data");
            
            // Verificar columna 4 (columna E)
            Column column = cells.CheckColumn(4);
            
            // Mostrar propiedades de la columna
            Console.WriteLine("Column Width: " + column.Width);
            Console.WriteLine("Column Index: " + column.Index);
        }
    }
}
```

### Ver también

* class [Column](../../column/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


