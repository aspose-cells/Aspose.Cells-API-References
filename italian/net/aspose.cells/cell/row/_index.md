---
title: "Cell.Row"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Restituisce il numero di riga zero basato sulla cella"
type: docs
url: /it/net/aspose.cells/cell/row/
---
## Cell.Row property

Ottiene il numero di riga (basato su zero) della cella.

```csharp
public int Row { get; }
```

### Property Value

Numero di riga della cella

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio e formula
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");
            
            // Trova la cella contenente la formula
            Cell cell = worksheet.Cells.Find("=SUM(A1", null, new FindOptions()
            { 
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.Contains 
            });
            
            // Dimostra la proprietà Row
            Console.WriteLine("Formula found in row: " + cell.Row);
            Console.WriteLine("Formula found in column: " + cell.Column);
            
            // Verifica che la riga sia corretta
            if (cell.Row == 2 && cell.Column == 0)
            {
                Console.WriteLine("Row property works correctly");
            }
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


