---
title: "Cells.CheckRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottiene l'elemento Row o null all'indice di riga della cella specificato"
type: docs
url: /it/net/aspose.cells/cells/checkrow/
---
## Cells.CheckRow method

Ottiene l'elemento [`Row`](../../row/) o null all'indice di riga della cella specificato.

```csharp
public Row CheckRow(int row)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice della riga |

### Valore di ritorno

Restituisce l'oggetto [`Row`](../../row/) se l'oggetto riga esiste, altrimenti restituisce null.

### Esempi

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
            
            // Popola alcuni dati
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue(100);
            cells["A3"].PutValue(200);
            
            // Verifica se la riga esiste e ottieni l'oggetto riga
            Row row = cells.CheckRow(1);
            if (row != null)
            {
                Console.WriteLine("Row 1 exists with height: " + row.Height);
            }
            
            // Verifica riga inesistente
            Row nonExistentRow = cells.CheckRow(100);
            Console.WriteLine("Row 100 exists: " + (nonExistentRow != null));
        }
    }
}
```

### Vedi anche

* class [Row](../../row/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


