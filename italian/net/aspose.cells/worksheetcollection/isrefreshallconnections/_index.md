---
title: "WorksheetCollection.IsRefreshAllConnections"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorksheetCollection. Indica se rinfrescare tutte le connessioni all'apertura del file in MS Excel"
type: docs
url: /it/net/aspose.cells/worksheetcollection/isrefreshallconnections/
---
## WorksheetCollection.IsRefreshAllConnections property

Indica se aggiornare tutte le connessioni all'apertura del file in MS Excel.

```csharp
public bool IsRefreshAllConnections { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyIsRefreshAllConnectionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alla collezione di fogli di lavoro
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // Aggiungi alcuni fogli di lavoro di esempio
            worksheets.Add("Sheet1");
            worksheets.Add("Sheet2");
            
            // Imposta la proprietà IsRefreshAllConnections
            worksheets.IsRefreshAllConnections = true;
            
            // Visualizza il valore corrente di IsRefreshAllConnections
            Console.WriteLine("IsRefreshAllConnections: " + worksheets.IsRefreshAllConnections);
            
            // Salva la cartella di lavoro
            workbook.Save("WorksheetCollectionPropertyIsRefreshAllConnectionsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


