---
title: "CellsHelper.RowIndexToName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CellsHelper. Ottiene il nome della riga in base all'indice della riga"
type: docs
url: /it/net/aspose.cells/cellshelper/rowindextoname/
---
## CellsHelper.RowIndexToName method

Ottiene il nome della riga in base all'indice della riga.

```csharp
public static string RowIndexToName(int row)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice della riga. |

### Valore di ritorno

Nome della riga.

### Esempi

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

### Vedi anche

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


