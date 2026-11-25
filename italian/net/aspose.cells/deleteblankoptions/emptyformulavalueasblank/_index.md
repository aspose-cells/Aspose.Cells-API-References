---
title: "DeleteBlankOptions.EmptyFormulaValueAsBlank"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DeleteBlankOptions. Indica se una cella verrà considerata vuota quando è una formula e il risultato calcolato è null o una stringa vuota. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/deleteblankoptions/emptyformulavalueasblank/
---
## DeleteBlankOptions.EmptyFormulaValueAsBlank property

Se una cella verrà considerata vuota quando è una formula e il risultato calcolato è null o stringa vuota. Il valore predefinito è false.

```csharp
public bool EmptyFormulaValueAsBlank { get; set; }
```

### Osservazioni

In generale l'utente dovrebbe assicurarsi che le formule siano state calcolate prima dell'operazione di eliminazione con questa proprietà impostata su true. Altrimenti tutte le nuove formule create dalle API normali, come [`Formula`](../../cell/formula/), saranno considerate vuote e potrebbero essere eliminate perché, prima del calcolo, i loro risultati calcolati sono tutti null.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEmptyFormulaValueAsBlankDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Popola dati di esempio
            cells["A1"].PutValue("Header");
            cells["A2"].Formula = "=B2";  // Formula returning blank
            cells["A3"].PutValue("Data");
            cells["A4"].Formula = "=1+1"; // Formula with value
            
            // Elimina le righe vuote senza considerare i vuoti delle formule
            Console.WriteLine("Before deletion (normal): " + cells.MaxRow + " rows");
            cells.DeleteBlankRows();
            Console.WriteLine("After normal deletion: " + cells.MaxRow + " rows");

            // Reimposta i dati
            cells.ClearContents(0, 0, cells.MaxRow + 1, cells.MaxColumn + 1);
            cells["A1"].PutValue("Header");
            cells["A2"].Formula = "=B2";
            cells["A3"].PutValue("Data");
            cells["A4"].Formula = "=1+1";

            // Elimina le righe vuote trattando i vuoti delle formule come vuoti
            Console.WriteLine("\nBefore deletion (with EmptyFormulaValueAsBlank): " + cells.MaxRow + " rows");
            cells.DeleteBlankRows(new DeleteBlankOptions() { EmptyFormulaValueAsBlank = true });
            Console.WriteLine("After deletion with EmptyFormulaValueAsBlank: " + cells.MaxRow + " rows");
        }
    }
}
```

### Vedi anche

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


