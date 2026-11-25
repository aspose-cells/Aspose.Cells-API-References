---
title: "Row.GetCellByIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Row. Ottieni la cella tramite un indice specifico nella collezione di celle di questa riga"
type: docs
url: /it/net/aspose.cells/row/getcellbyindex/
---
## Row.GetCellByIndex method

Ottieni la cella tramite indice specifico nella collezione di celle di questa riga.

```csharp
public Cell GetCellByIndex(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice (posizione) della cella nella collezione di celle di questa riga. |

### Valore di ritorno

L'oggetto Cell nella posizione indicata.

### Osservazioni

Per attraversare tutte le celle in sequenza senza modificarle, usare [`GetEnumerator`](../getenumerator/) offrirà prestazioni migliori rispetto all'utilizzo di questo metodo per ottenere le celle una alla volta.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetCellByIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati alle celle nella prima riga
            worksheet.Cells["A1"].PutValue("Cell A1");
            worksheet.Cells["B1"].PutValue("Cell B1");
            worksheet.Cells["C1"].PutValue("Cell C1");

            // Ottieni la prima riga
            Row row = worksheet.Cells.Rows[0];

            // Dimostra GetCellByIndex con parametro Int32
            Cell cellAtIndex0 = row.GetCellByIndex(0);
            Cell cellAtIndex1 = row.GetCellByIndex(1);
            Cell cellAtIndex2 = row.GetCellByIndex(2);

            Console.WriteLine("Cell at index 0: " + cellAtIndex0.StringValue);
            Console.WriteLine("Cell at index 1: " + cellAtIndex1.StringValue);
            Console.WriteLine("Cell at index 2: " + cellAtIndex2.StringValue);

            workbook.Save("RowGetCellByIndexDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


