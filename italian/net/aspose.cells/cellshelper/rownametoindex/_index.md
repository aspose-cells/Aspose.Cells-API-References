---
title: "CellsHelper.RowNameToIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CellsHelper. Ottiene l'indice della riga in base al nome della riga"
type: docs
url: /it/net/aspose.cells/cellshelper/rownametoindex/
---
## CellsHelper.RowNameToIndex method

Ottiene l'indice della riga in base al nome della riga.

```csharp
public static int RowNameToIndex(string rowName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowName | String | Nome della riga. |

### Valore di ritorno

Indice della riga.

### Esempi

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

### Vedi anche

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


