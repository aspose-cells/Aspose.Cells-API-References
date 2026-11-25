---
title: "Worksheet.SelectRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Seleziona un intervallo"
type: docs
url: /it/net/aspose.cells/worksheet/selectrange/
---
## Worksheet.SelectRange method

Seleziona un intervallo.

```csharp
public void SelectRange(int startRow, int startColumn, int totalRows, int totalColumns, 
    bool removeOthers)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | La riga iniziale. |
| startColumn | Int32 | La colonna iniziale |
| totalRows | Int32 | Il numero di righe. |
| totalColumns | Int32 | Il numero di colonne |
| removeOthers | Booleano | True indica la rimozione di altri intervalli selezionati e la selezione solo di questo intervallo. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodSelectRangeWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Seleziona l'intervallo dalla riga 1, colonna 1 alla riga 5, colonna 5 (B2:F6) e rendilo attivo
            worksheet.SelectRange(1, 1, 5, 5, true);
            
            Console.WriteLine("Active cell: " + worksheet.ActiveCell);
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


