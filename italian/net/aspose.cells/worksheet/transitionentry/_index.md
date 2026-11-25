---
title: "Worksheet.TransitionEntry"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Indica se l'opzione di compatibilità Lotus per Transition Formula Entry è abilitata"
type: docs
url: /it/net/aspose.cells/worksheet/transitionentry/
---
## Worksheet.TransitionEntry property

Indica se l'opzione Transition Formula Entry (compatibilità Lotus) è abilitata.

```csharp
public bool TransitionEntry { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTransitionEntryDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta la proprietà TransitionEntry
            worksheet.TransitionEntry = true;
            
            // Visualizza il valore di TransitionEntry
            Console.WriteLine("TransitionEntry: " + worksheet.TransitionEntry);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            // Carica la cartella di lavoro salvata per verificare la proprietà
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Visualizza il valore di TransitionEntry caricato
            Console.WriteLine("Loaded TransitionEntry: " + loadedWorksheet.TransitionEntry);
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


