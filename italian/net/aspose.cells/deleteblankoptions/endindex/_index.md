---
title: "DeleteBlankOptions.EndIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DeleteBlankOptions. Specifica l'indice finale di riga/colonna inclusivo dell'intervallo da controllare e cancellare righe/colonne vuote. Il valore predefinito è 1 e 1 indica l'intervallo massimo di tutti gli oggetti celle disegni ... che devono essere controllati"
type: docs
url: /it/net/aspose.cells/deleteblankoptions/endindex/
---
## DeleteBlankOptions.EndIndex property

Specifica l'indice di riga/colonna finale (inclusivo) dell'intervallo da controllare e cancellare righe/colonne vuote. Il valore predefinito è -1 e -1 indica l'intervallo massimo di tutti gli oggetti (celle, disegni, ...) che devono essere controllati.

```csharp
public int EndIndex { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEndIndexDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Popola alcune celle con valori
            cells[0, 2].PutValue(2);
            cells[0, 5].PutValue(5);
            cells[0, 9].PutValue(9);

            // Crea opzioni di cancellazione con un intervallo specifico
            DeleteBlankOptions dbo = new DeleteBlankOptions();
            dbo.StartIndex = 4;
            dbo.EndIndex = 7;

            // Elimina colonne vuote all'interno dell'intervallo specificato
            cells.DeleteBlankColumns(dbo);

            // Genera output dei risultati per dimostrare l'effetto di EndIndex
            Console.WriteLine("Value at C1: " + cells[0, 2].IntValue);
            Console.WriteLine("Value at F1 (originally G1): " + cells[0, 4].IntValue);
            Console.WriteLine("Value at G1 (originally K1): " + cells[0, 6].IntValue);
        }
    }
}
```

### Vedi anche

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


