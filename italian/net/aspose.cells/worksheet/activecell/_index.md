---
title: "Worksheet.ActiveCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottiene o imposta la cella attiva nel foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/activecell/
---
## Worksheet.ActiveCell property

Ottiene o imposta la cella attiva nel foglio di lavoro.

```csharp
public string ActiveCell { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyActiveCellDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta la cella attiva su B2
            worksheet.ActiveCell = "B2";
            
            // Stampa l'indirizzo della cella attiva
            Console.WriteLine("Active Cell: " + worksheet.ActiveCell);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            // Carica la cartella di lavoro salvata per verificare la cella attiva
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Loaded Active Cell: " + loadedWorkbook.Worksheets[0].ActiveCell);
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


