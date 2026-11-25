---
title: "Cells.MinDataColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Indice minimo della colonna della cella che contiene dati"
type: docs
url: /it/net/aspose.cells/cells/mindatacolumn/
---
## Cells.MinDataColumn property

Indice di colonna minimo della cella che contiene dati.

```csharp
public int MinDataColumn { get; }
```

### Osservazioni

-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinDataColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Aggiungi alcuni dati alle celle (a partire dalla colonna 2)
            cells["B1"].PutValue("Header1");
            cells["C2"].PutValue("Data1");
            cells["D3"].PutValue("Data2");
            cells["E4"].PutValue("Data3");
            
            // Ottieni l'indice di colonna minimo che contiene dati
            int minDataColumn = cells.MinDataColumn;
            
            // Restituisci il risultato
            Console.WriteLine("Minimum data column index: " + minDataColumn);
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


