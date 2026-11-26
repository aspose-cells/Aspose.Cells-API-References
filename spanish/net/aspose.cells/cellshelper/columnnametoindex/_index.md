---
title: "CellsHelper.ColumnNameToIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CellsHelper. Obtiene el índice de columna según el nombre de la columna"
type: docs
url: /es/net/aspose.cells/cellshelper/columnnametoindex/
---
## CellsHelper.ColumnNameToIndex method

Obtiene el índice de columna según el nombre de columna.

```csharp
public static int ColumnNameToIndex(string columnName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnName | String | Nombre de columna. |

### Valor de retorno

Índice de columna.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodColumnNameToIndexWithStringDemo
    {
        public static void Run()
        {
            int columnIndex = CellsHelper.ColumnNameToIndex("BAA");
            string columnName = CellsHelper.ColumnIndexToName(columnIndex);
            
            Console.WriteLine("Column Name: " + columnName);
            Console.WriteLine("Column Index: " + columnIndex);
        }
    }
}
```

### Ver también

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


