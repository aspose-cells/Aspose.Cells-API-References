---
title: "CellArea.StartColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Campo CellArea. Ottiene o imposta la colonna iniziale di quest'area"
type: docs
url: /it/net/aspose.cells/cellarea/startcolumn/
---
## CellArea.StartColumn field

Ottiene o imposta la colonna iniziale di quest'area.

```csharp
public int StartColumn;
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaFieldStartColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta alcuni dati iniziali
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue(10);
            cells["A3"].PutValue(20);

            // Crea un CellArea e imposta la sua StartColumn
            CellArea area = new CellArea();
            area.StartRow = 1;
            area.EndRow = 3;
            area.StartColumn = 0; // Using StartColumn field
            area.EndColumn = 0;

            // Inserisci una nuova colonna spostando le celle esistenti verso il basso
            cells.InsertRange(area, ShiftType.Down);

            // Verifica il risultato
            Console.WriteLine("A1 value: " + cells["A1"].StringValue); // Should be empty
            Console.WriteLine("A2 value: " + cells["A2"].StringValue); // Should be "Header"
            Console.WriteLine("A3 value: " + cells["A3"].IntValue); // Should be 10
        }
    }
}
```

### Vedi anche

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


