---
title: "Worksheet.PivotTables"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottiene tutte le tabelle pivot in questo foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/pivottables/
---
## Worksheet.PivotTables property

Ottiene tutte le tabelle pivot in questo foglio di lavoro.

```csharp
public PivotTableCollection PivotTables { get; }
```

### Esempi

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPivotTablesDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook("PivotTableExample.xlsx");
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla raccolta di tabelle pivot dal foglio di lavoro
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Verifica se ci sono tabelle pivot
            if (pivotTables.Count > 0)
            {
                // Ottieni la prima tabella pivot
                PivotTable pivotTable = pivotTables[0];
                
                // Cancella eventuali filtri esistenti
                pivotTable.PivotFilters.Clear();
                
                // Aggiorna i dati della tabella pivot
                pivotTable.RefreshData();
                pivotTable.CalculateData();
                
                // Salva la cartella di lavoro modificata
                workbook.Save("PivotTableModified.xlsx");
            }
        }
    }
}
```

### Vedi anche

* class [PivotTableCollection](../../../aspose.cells.pivot/pivottablecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


