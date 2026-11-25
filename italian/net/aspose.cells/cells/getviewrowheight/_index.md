---
title: "Cells.GetViewRowHeight"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottiene l'altezza di una riga specificata"
type: docs
url: /it/net/aspose.cells/cells/getviewrowheight/
---
## Cells.GetViewRowHeight method

Restituisce l'altezza di una riga specificata.

```csharp
public double GetViewRowHeight(int row)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice della riga. |

### Valore di ritorno

Altezza della riga.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetViewRowHeightWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta l'altezza della riga per la riga 3 (in punti)
            worksheet.Cells.SetRowHeight(3, 15);
            
            // Ottieni l'altezza visualizzata della riga per la riga 3
            double viewRowHeight = worksheet.Cells.GetViewRowHeight(3);
            
            // Restituisci il risultato
            Console.WriteLine("View Row Height for row 3: " + viewRowHeight);
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


