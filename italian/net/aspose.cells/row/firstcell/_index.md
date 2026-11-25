---
title: "Row.FirstCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Row proprietà. Restituisce il primo oggetto cella nella riga"
type: docs
url: /it/net/aspose.cells/row/firstcell/
---
## Row.FirstCell property

Ottiene il primo oggetto cella nella riga.

```csharp
public Cell FirstCell { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyFirstCellDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati alle celle nella prima riga
            worksheet.Cells["A1"].PutValue("First Cell");
            worksheet.Cells["B1"].PutValue("Second Cell");
            worksheet.Cells["C1"].PutValue("Third Cell");
            
            // Ottieni la prima riga
            Row row = worksheet.Cells.Rows[0];
            
            // Dimostra la proprietà FirstCell
            Cell firstCell = row.FirstCell;
            Console.WriteLine("First cell in row: " + firstCell.Name + " with value: " + firstCell.StringValue);
            
            // Modifica la prima cella
            firstCell.PutValue("Modified First Cell");
            Console.WriteLine("Updated first cell value: " + firstCell.StringValue);
            
            // Salva la cartella di lavoro
            workbook.Save("RowFirstCellDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


