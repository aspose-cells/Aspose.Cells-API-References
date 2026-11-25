---
title: "RevisionCellComment.IsOldComment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionCellComment. Indica se è un commento vecchio"
type: docs
url: /it/net/aspose.cells.revisions/revisioncellcomment/isoldcomment/
---
## RevisionCellComment.IsOldComment property

Indica se è un commento precedente.

```csharp
public bool IsOldComment { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyIsOldCommentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con tracciamento delle revisioni
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi il commento iniziale alla cella A1
            Comment comment = worksheet.Comments[0, 0];
            comment.Note = "First version of comment";

            // Modifica il commento per generare una revisione
            comment.Note = "Updated comment text";

            // Aggiungi un altro commento alla cella B2
            Comment secondComment = worksheet.Comments[1, 1];
            secondComment.Note = "Second comment";

            // Accedi alle revisioni
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Visualizza il valore della proprietà IsOldComment
                    Console.WriteLine("Cell: " + commentRevision.CellName);
                    Console.WriteLine("IsOldComment: " + commentRevision.IsOldComment);
                    
                    // Dimostra l'uso della proprietà IsOldComment
                    if (commentRevision.IsOldComment)
                    {
                        Console.WriteLine("This revision represents the old state of the comment");
                        Console.WriteLine("Old comment length: " + commentRevision.OldLength);
                    }
                    else
                    {
                        Console.WriteLine("This revision represents the new state of the comment");
                        Console.WriteLine("New comment length: " + commentRevision.NewLength);
                    }

                    // Mostra le proprietà correlate
                    Console.WriteLine("Action Type: " + commentRevision.ActionType);
                    Console.WriteLine("Revision Type: " + commentRevision.Type);
                }
            }

            // Salva la cartella di lavoro con le revisioni
            workbook.Save("RevisionCellCommentPropertyIsOldCommentDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


