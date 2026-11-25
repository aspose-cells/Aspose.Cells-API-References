---
title: "CellsHelper.ColumnNameToIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CellsHelper. Ottiene l'indice di colonna in base al nome della colonna"
type: docs
url: /it/net/aspose.cells/cellshelper/columnnametoindex/
---
## CellsHelper.ColumnNameToIndex method

Ottiene l'indice della colonna in base al nome della colonna.

```csharp
public static int ColumnNameToIndex(string columnName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnName | String | Nome colonna. |

### Valore di ritorno

Indice colonna.

### Esempi

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

### Vedi anche

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


