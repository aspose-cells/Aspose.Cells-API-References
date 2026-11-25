---
title: "RevisionLog.Revisions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionLog. Ottiene tutte le revisioni in questo registro"
type: docs
url: /it/net/aspose.cells.revisions/revisionlog/revisions/
---
## RevisionLog.Revisions property

Ottiene tutte le revisioni in questo log.

```csharp
public RevisionCollection Revisions { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionLogPropertyRevisionsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con la cronologia delle revisioni
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Apporta alcune modifiche per tenere traccia delle revisioni
            worksheet.Cells["A1"].PutValue("Initial Value");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].Formula = "=A2*2";
            
            // Salva con il tracciamento delle revisioni
            workbook.Save("revision_demo.xlsx", SaveFormat.Xlsx);
            
            // Apporta altre modifiche per creare revisioni
            worksheet.Cells["A1"].PutValue("Modified Value");
            worksheet.Cells["A2"].PutValue(200);
            
            // Salva di nuovo per registrare le revisioni
            workbook.Save("revision_demo.xlsx", SaveFormat.Xlsx);
            
            // Carica la cartella di lavoro con le revisioni
            Workbook workbookWithRevisions = new Workbook("revision_demo.xlsx");
            
            // Accedi ai log delle revisioni
            RevisionLogCollection revisionLogs = workbookWithRevisions.Worksheets.RevisionLogs;
            
            // Elabora ogni registro delle revisioni
            foreach (RevisionLog log in revisionLogs)
            {
                Console.WriteLine($"Processing revision log with {log.Revisions.Count} revisions");
                
                // Accedi alla raccolta delle revisioni
                RevisionCollection revisions = log.Revisions;
                
                foreach (Revision revision in revisions)
                {
                    Console.WriteLine($"Revision Type: {revision.Type}");
                    
                    if (revision.Type == RevisionType.ChangeCells)
                    {
                        RevisionCellChange cellChange = (RevisionCellChange)revision;
                        Console.WriteLine($"Cell {cellChange.CellName} changed from '{cellChange.OldValue}' to '{cellChange.NewValue}'");
                    }
                }
            }
        }
    }
}
```

### Vedi anche

* class [RevisionCollection](../../revisioncollection/)
* class [RevisionLog](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


