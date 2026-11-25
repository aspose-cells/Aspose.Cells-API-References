---
title: "RevisionLogCollection.DaysPreservingHistory"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionLogCollection. Ottiene e imposta il numero di giorni per cui l'applicazione di foglio di calcolo manterrà la cronologia delle modifiche per questa cartella di lavoro"
type: docs
url: /it/net/aspose.cells.revisions/revisionlogcollection/dayspreservinghistory/
---
## RevisionLogCollection.DaysPreservingHistory property

Ottiene e imposta il numero di giorni in cui l'applicazione di foglio di calcolo manterrà la cronologia delle modifiche per questa cartella di lavoro.

```csharp
public int DaysPreservingHistory { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RevisionLogCollectionPropertyDaysPreservingHistoryDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Value");
            
            // Imposta la proprietà DaysPreservingHistory
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 40;
            
            string outputPath = "output_DaysPreservingHistory.xlsx";
            workbook.Save(outputPath);
            
            // Ricarica per verificare la proprietà
            Workbook loadedWorkbook = new Workbook(outputPath);
            Console.WriteLine("DaysPreservingHistory: " + 
                loadedWorkbook.Worksheets.RevisionLogs.DaysPreservingHistory);
        }
    }
}
```

### Vedi anche

* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


