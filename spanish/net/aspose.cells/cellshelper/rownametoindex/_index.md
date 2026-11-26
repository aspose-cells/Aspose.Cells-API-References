---
title: "CellsHelper.RowNameToIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CellsHelper. Obtiene el índice de fila según el nombre de fila"
type: docs
url: /es/net/aspose.cells/cellshelper/rownametoindex/
---
## CellsHelper.RowNameToIndex method

Obtiene el índice de fila según el nombre de fila.

```csharp
public static int RowNameToIndex(string rowName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowName | String | Nombre de fila. |

### Valor de retorno

Índice de fila.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodRowNameToIndexWithStringDemo
    {
        public static void Run()
        {
            string rowName = "11";
            int rowIndex = CellsHelper.RowNameToIndex(rowName);
            Console.WriteLine("Row name '{0}' converted to index: {1}", rowName, rowIndex);
        }
    }
}
```

### Ver también

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


