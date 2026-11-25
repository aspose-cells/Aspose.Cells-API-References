---
title: "Style.IsTextWrapped"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Ottiene o imposta un valore che indica se il testo all'interno di una cella è a capo"
type: docs
url: /it/net/aspose.cells/style/istextwrapped/
---
## Style.IsTextWrapped property

Ottiene o imposta un valore che indica se il testo all'interno di una cella è a capo.

```csharp
public bool IsTextWrapped { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            Cells cells = ws.Cells;
            
            // Imposta testo lungo nella cella
            Cell cell = cells["A1"];
            cell.PutValue("This is a long text that should be wrapped in the cell");
            
            // Abilita l'andare a capo del testo
            Style style = cell.GetStyle();
            style.IsTextWrapped = true;
            cell.SetStyle(style);
            
            // Regola l'altezza della riga per mostrare il testo a capo
            ws.AutoFitRow(0);
            
            // Salva la cartella di lavoro
            wb.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


