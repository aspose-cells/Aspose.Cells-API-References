---
title: "RevisionLog.Revisions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionLog-Eigenschaft. Gibt alle Revisionen in diesem Protokoll zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisionlog/revisions/
---
## RevisionLog.Revisions property

Ermittelt alle Revisionen in diesem Protokoll.

```csharp
public RevisionCollection Revisions { get; }
```

### Beispiele

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
            // Erstellen Sie eine Arbeitsmappe mit Revisionsverlauf
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Nehmen Sie einige Änderungen vor, um Revisionen zu verfolgen
            worksheet.Cells["A1"].PutValue("Initial Value");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].Formula = "=A2*2";
            
            // Speichern Sie mit Revisionsverfolgung
            workbook.Save("revision_demo.xlsx", SaveFormat.Xlsx);
            
            // Nehmen Sie weitere Änderungen vor, um Revisionen zu erzeugen
            worksheet.Cells["A1"].PutValue("Modified Value");
            worksheet.Cells["A2"].PutValue(200);
            
            // Speichern Sie erneut, um Revisionen zu protokollieren
            workbook.Save("revision_demo.xlsx", SaveFormat.Xlsx);
            
            // Laden Sie die Arbeitsmappe mit Revisionen
            Workbook workbookWithRevisions = new Workbook("revision_demo.xlsx");
            
            // Zugriff auf Revisionsprotokolle
            RevisionLogCollection revisionLogs = workbookWithRevisions.Worksheets.RevisionLogs;
            
            // Verarbeiten Sie jedes Revisionsprotokoll
            foreach (RevisionLog log in revisionLogs)
            {
                Console.WriteLine($"Processing revision log with {log.Revisions.Count} revisions");
                
                // Greifen Sie auf die Revisionssammlung zu
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

### Siehe auch

* class [RevisionCollection](../../revisioncollection/)
* class [RevisionLog](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


