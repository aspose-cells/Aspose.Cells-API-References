---
title: "Cells.CheckColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottiene l'elemento Column o null all'indice colonna specificato"
type: docs
url: /it/net/aspose.cells/cells/checkcolumn/
---
## Cells.CheckColumn method

Ottiene l'elemento [`Column`](../../column/) o null all'indice colonna specificato.

```csharp
public Column CheckColumn(int columnIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | Int32 | L'indice della colonna. |

### Valore di ritorno

L'oggetto Column.

### Esempi

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
            
            // Imposta un valore nella colonna 1 (B3)
            cells["B3"].PutValue("Sample Data");
            
            // Verifica colonna 4 (colonna E)
            Column column = cells.CheckColumn(4);
            
            // Proprietà della colonna di output
            Console.WriteLine("Column Width: " + column.Width);
            Console.WriteLine("Column Index: " + column.Index);
        }
    }
}
```

### Vedi anche

* class [Column](../../column/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


