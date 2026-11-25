---
title: "Cells.MaxColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Indice di colonna massimo di quelle celle che sono state istanziate nella raccolta non include la colonna in cui lo stile è definito per l'intera colonna ma nessuna cella è stata istanziata in essa"
type: docs
url: /it/net/aspose.cells/cells/maxcolumn/
---
## Cells.MaxColumn property

Indice di colonna massimo delle celle che sono state istanziate nella raccolta (non include la colonna in cui lo stile è definito per l'intera colonna ma non è stata istanziata alcuna cella).

```csharp
public int MaxColumn { get; }
```

### Osservazioni

Restituisci -1 se non è stata istanziata alcuna cella.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati alle celle
            worksheet.Cells["A1"].PutValue("Column A");
            worksheet.Cells["B1"].PutValue("Column B");
            worksheet.Cells["C1"].PutValue("Column C");
            
            // Ottieni l'indice di colonna massimo con dati
            int maxColumn = worksheet.Cells.MaxColumn;
            Console.WriteLine("Max column with data: " + maxColumn);

            // Aggiungi dati alla colonna successiva dopo la colonna massima
            worksheet.Cells[0, maxColumn + 1].PutValue("Next Column");

            // Verifica la nuova colonna massima
            Console.WriteLine("New max column: " + worksheet.Cells.MaxColumn);

            // Crea un altro foglio di lavoro per dimostrare la copia
            Worksheet destSheet = workbook.Worksheets.Add("Destination");

            // Copia tutte le colonne dalla sorgente alla destinazione
            destSheet.Cells.CopyColumns(worksheet.Cells, 0, 0, worksheet.Cells.MaxColumn + 1);

            Console.WriteLine("Columns copied successfully");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


