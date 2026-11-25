---
title: "Cells.CopyColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Copia dati e formati di un'intera colonna"
type: docs
url: /it/net/aspose.cells/cells/copycolumn/
---
## Cells.CopyColumn method

Copia i dati e i formati di un'intera colonna.

```csharp
public void CopyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceCells | Celle | L'oggetto Source Cells contiene dati e formati da copiare. |
| sourceColumnIndex | Int32 | Indice della colonna di origine. |
| destinationColumnIndex | Int32 | Indice della colonna di destinazione. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyColumnWithCellsInt32Int32Demo
    {
        public static void Run()
        {
            // Crea la cartella di lavoro di origine e popola i dati
            Workbook wbSrc = new Workbook();
            Cells cellsSrc = wbSrc.Worksheets[0].Cells;
            cellsSrc[0, 255].PutValue(1);
            cellsSrc[1, 255].PutValue(true);
            cellsSrc[2, 255].PutValue("abc");
            cellsSrc[3, 255].PutValue(false);
            cellsSrc[65535, 255].PutValue(2.56);

            // Crea la cartella di lavoro di destinazione
            Workbook wbDest = new Workbook();
            Cells cellsDest = wbDest.Worksheets[0].Cells;

            // Copia la colonna dalla sorgente alla destinazione
            cellsDest.CopyColumn(cellsSrc, 255, 0);

            // Salva il risultato
            wbDest.Save("outputCopyColumn.xlsx");
            
            Console.WriteLine("Column copied successfully.");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


