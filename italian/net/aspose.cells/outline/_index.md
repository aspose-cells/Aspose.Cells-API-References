---
title: "Classe Outline"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Outline. Rappresenta una struttura di riepilogo in un foglio di lavoro"
type: docs
url: /it/net/aspose.cells/outline/
---
## Outline class

Rappresenta una struttura su un foglio di lavoro.

```csharp
public class Outline
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [SummaryColumnRight](../../aspose.cells/outline/summarycolumnright/) { get; set; } | Indica se la colonna di riepilogo sarà posizionata a destra delle colonne di dettaglio nella struttura. |
| [SummaryRowBelow](../../aspose.cells/outline/summaryrowbelow/) { get; set; } | Indica se la riga di riepilogo sarà posizionata sotto le righe di dettaglio nella struttura. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OutlineDemo
    {
        public static void OutlineExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro nella cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla struttura del foglio di lavoro
            Outline outline = worksheet.Outline;
            
            // Imposta le proprietà della struttura
            outline.SummaryRowBelow = true; // Indicates if the summary row will be positioned below the detail rows
            outline.SummaryColumnRight = true; // Indicates if the summary column will be positioned to the right of the detail columns
            
            // Salva la cartella di lavoro
            workbook.Save("OutlineExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


