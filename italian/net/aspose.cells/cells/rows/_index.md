---
title: "Cells.Rows"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Ottiene la collezione di oggetti Row che rappresentano le singole righe in questo foglio di lavoro"
type: docs
url: /it/net/aspose.cells/cells/rows/
---
## Cells.Rows property

Ottiene la collezione di oggetti [`Row`](../../row/) che rappresentano le singole righe in questo foglio di lavoro.

```csharp
public RowCollection Rows { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyRowsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta la larghezza della colonna e l'altezza della riga
            worksheet.Cells.SetColumnWidthPixel(0, 200);
            worksheet.Cells.Rows[0].Height = 50;
            
            // Accedi alle proprietà della riga tramite la collezione Rows
            Row row = worksheet.Cells.Rows[0];
            Console.WriteLine($"Row 0 height: {row.Height}");
            Console.WriteLine($"Is height matched: {row.IsHeightMatched}");
            
            // Modifica le proprietà della riga
            row.IsHeightMatched = true;
            row.Height = 60;
            
            // Verifica le modifiche
            Console.WriteLine($"Modified row 0 height: {worksheet.Cells.GetRowHeightPixel(0)}");
            Console.WriteLine($"Is height matched after change: {row.IsHeightMatched}");
            
            // Salva la cartella di lavoro
            workbook.Save("CellsPropertyRowsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [RowCollection](../../rowcollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


