---
title: "Cells.GetRowHeightInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Restituisce l'altezza di una riga specificata nell'unità di pollici"
type: docs
url: /it/net/aspose.cells/cells/getrowheightinch/
---
## Cells.GetRowHeightInch method

Restituisce l'altezza di una riga specificata in unità di pollici.

```csharp
public double GetRowHeightInch(int row)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice della riga |

### Valore di ritorno

Altezza della riga

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetRowHeightInchWithInt32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta l'altezza della riga in pollici per la riga 5
            cells.SetRowHeightInch(5, 1.5);

            // Ottieni l'altezza della riga in pollici per la riga 5
            double rowHeight = cells.GetRowHeightInch(5);

            // Restituisci il risultato
            Console.WriteLine("Row height in inches: " + rowHeight);
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


