---
title: "CellsHelper.RowIndexToName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CellsHelper. Obtiene el nombre de la fila según el índice de fila"
type: docs
url: /es/net/aspose.cells/cellshelper/rowindextoname/
---
## CellsHelper.RowIndexToName method

Obtiene el nombre de fila según el índice de fila.

```csharp
public static string RowIndexToName(int row)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila. |

### Valor de retorno

Nombre de la fila.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodRowIndexToNameWithInt32Demo
    {
        public static void Run()
        {
            int rowIndex = 10;
            string rowName = CellsHelper.RowIndexToName(rowIndex);
            Console.WriteLine("Row index {0} corresponds to row name: {1}", rowIndex, rowName);
            
            int convertedBackIndex = CellsHelper.RowNameToIndex(rowName);
            Console.WriteLine("Row name {0} converted back to index: {1}", rowName, convertedBackIndex);
        }
    }
}
```

### Ver también

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


