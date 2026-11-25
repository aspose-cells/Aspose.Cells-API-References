---
title: "CellWatch.Row"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CellWatch. Restituisce e imposta la riga della cella"
type: docs
url: /it/net/aspose.cells/cellwatch/row/
---
## CellWatch.Row property

Ottiene e imposta la riga della cella.

```csharp
public int Row { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchPropertyRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio alla cella B2
            sheet.Cells["B2"].PutValue("Sample Data");

            // Aggiungi CellWatch per B2
            int watchIndex = sheet.CellWatches.Add("B2");
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // Dimostra la proprietà Row
            Console.WriteLine($"Original Row: {cellWatch.Row}");
            cellWatch.Row = 1; // Set row to 1 (0-based) for B2
            Console.WriteLine($"Updated Row: {cellWatch.Row}");

            // Verifica il riferimento della cella
            Console.WriteLine($"Cell Reference: {sheet.Cells[cellWatch.Row, cellWatch.Column].Name}");

            workbook.Save("CellWatchRowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


