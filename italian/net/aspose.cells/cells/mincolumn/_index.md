---
title: "Cells.MinColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Indice di colonna minimo di quelle celle che sono state istanziate nella raccolta non include la colonna in cui lo stile è definito per l'intera colonna ma nessuna cella è stata istanziata in essa"
type: docs
url: /it/net/aspose.cells/cells/mincolumn/
---
## Cells.MinColumn property

Indice di colonna minimo delle celle che sono state istanziate nella raccolta (non include la colonna in cui lo stile è definito per l'intera colonna ma non è stata istanziata alcuna cella).

```csharp
public int MinColumn { get; }
```

### Osservazioni

Questa proprietà deve iterare e controllare celle e righe in modo dinamico, quindi è un processo che richiede tempo e non dovrebbe essere invocata ripetutamente, ad esempio usandola direttamente come condizione in un ciclo.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla collezione di celle
            Cells cells = worksheet.Cells;
            
            // Popola alcuni dati nelle colonne 2, 3 e 4 (B, C, D)
            cells["B1"].PutValue("Data in Column B");
            cells["C1"].PutValue("Data in Column C");
            cells["D1"].PutValue("Data in Column D");
            
            // Ottieni l'indice di colonna minimo che contiene dati
            int minColumn = cells.MinColumn;
            
            // Ottieni l'indice di colonna massimo che contiene dati
            int maxColumn = cells.MaxColumn;
            
            Console.WriteLine("Minimum column with data: " + minColumn); // Should output 1 (column B)
            Console.WriteLine("Maximum column with data: " + maxColumn); // Should output 3 (column D)
            
            // Cancella la colonna B per dimostrare la modifica di MinColumn
            cells.DeleteColumn(1);
            
            Console.WriteLine("\nAfter deleting column B:");
            Console.WriteLine("New minimum column with data: " + cells.MinColumn); // Should now output 2 (column C)
            Console.WriteLine("Maximum column with data: " + cells.MaxColumn); // Should still output 3 (column D)
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


