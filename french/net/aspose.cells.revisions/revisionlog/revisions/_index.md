---
title: "RevisionLog.Revisions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionLog. Obtient toutes les révisions de ce journal"
type: docs
url: /fr/net/aspose.cells.revisions/revisionlog/revisions/
---
## RevisionLog.Revisions property

Obtient toutes les révisions de ce journal.

```csharp
public RevisionCollection Revisions { get; }
```

### Exemples

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
            // Créer un classeur avec l'historique des révisions
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Apporter quelques modifications pour suivre les révisions
            worksheet.Cells["A1"].PutValue("Initial Value");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].Formula = "=A2*2";
            
            // Enregistrer avec le suivi des révisions
            workbook.Save("revision_demo.xlsx", SaveFormat.Xlsx);
            
            // Apporter plus de modifications pour créer des révisions
            worksheet.Cells["A1"].PutValue("Modified Value");
            worksheet.Cells["A2"].PutValue(200);
            
            // Enregistrer à nouveau pour consigner les révisions
            workbook.Save("revision_demo.xlsx", SaveFormat.Xlsx);
            
            // Charger le classeur avec les révisions
            Workbook workbookWithRevisions = new Workbook("revision_demo.xlsx");
            
            // Accéder aux journaux de révision
            RevisionLogCollection revisionLogs = workbookWithRevisions.Worksheets.RevisionLogs;
            
            // Traiter chaque journal de révision
            foreach (RevisionLog log in revisionLogs)
            {
                Console.WriteLine($"Processing revision log with {log.Revisions.Count} revisions");
                
                // Accéder à la collection de révisions
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

### Voir aussi

* class [RevisionCollection](../../revisioncollection/)
* class [RevisionLog](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


