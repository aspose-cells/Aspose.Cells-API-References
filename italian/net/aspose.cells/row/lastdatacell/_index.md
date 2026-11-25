---
title: "Row.LastDataCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Row. Ottiene l'ultima cella non vuota nella riga"
type: docs
url: /it/net/aspose.cells/row/lastdatacell/
---
## Row.LastDataCell property

Ottiene l'ultima cella non vuota nella riga.

```csharp
public Cell LastDataCell { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyLastDataCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Inserisci dati nelle celle
            cells["A1"].PutValue("First cell");
            cells["B1"].PutValue("Second cell");
            cells["C2"].PutValue("Not in first row");
            
            // Ottieni l'ultima cella con dati nella prima riga
            Cell lastDataCell = cells.Rows[0].LastDataCell;
            
            Console.WriteLine("Last data cell in first row: " + lastDataCell.Name);
            Console.WriteLine("Value in last data cell: " + lastDataCell.StringValue);
        }
    }
}
```

### Vedi anche

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


