---
title: "Row.LastCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Row. Ottiene l'oggetto dell'ultima cella nella riga"
type: docs
url: /it/net/aspose.cells/row/lastcell/
---
## Row.LastCell property

Ottiene l'ultimo oggetto cella nella riga.

```csharp
public Cell LastCell { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyLastCellDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("First");
            worksheet.Cells["B1"].PutValue("Second");
            worksheet.Cells["C1"].PutValue("Last");

            // Ottieni la prima riga
            Row row = worksheet.Cells.Rows[0];

            // Accedi all'ultima cella nella riga
            Cell lastCell = row.LastCell;
            
            // Restituisci il valore dell'ultima cella
            Console.WriteLine("Last cell value: " + lastCell.Value);
        }
    }
}
```

### Vedi anche

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


