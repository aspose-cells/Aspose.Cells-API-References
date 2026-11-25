---
title: "RevisionCellComment.ActionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionCellComment. Restituisce il tipo di azione della revisione"
type: docs
url: /it/net/aspose.cells.revisions/revisioncellcomment/actiontype/
---
## RevisionCellComment.ActionType property

Ottiene il tipo di azione della revisione.

```csharp
public RevisionActionType ActionType { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyActionTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con tracciamento delle revisioni
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento alla cella A1
            Comment comment = worksheet.Comments[0, 0];
            comment.Note = "Initial comment";

            // Modifica il commento per generare una revisione
            comment.Note = "Updated comment";

            // Aggiungi un nuovo commento per generare una revisione di aggiunta
            Comment newComment = worksheet.Comments[1, 1];
            newComment.Note = "New comment";

            // Accedi alle revisioni
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Visualizza il valore della proprietà ActionType
                    Console.WriteLine("Revision ActionType: " + commentRevision.ActionType);
                    
                    // Dimostra l'uso della proprietà ActionType
                    switch (commentRevision.ActionType)
                    {
                        case RevisionActionType.Add:
                            Console.WriteLine("This revision added a new comment at " + commentRevision.CellName);
                            break;
                        case RevisionActionType.Delete:
                            Console.WriteLine("This revision deleted a comment from " + commentRevision.CellName);
                            break;
                        default:
                            Console.WriteLine("This revision modified a comment at " + commentRevision.CellName);
                            break;
                    }

                    // Mostra le proprietà correlate
                    Console.WriteLine("Comment location: " + commentRevision.CellName);
                    Console.WriteLine("Is old comment: " + commentRevision.IsOldComment);
                    Console.WriteLine("Old length: " + commentRevision.OldLength);
                    Console.WriteLine("New length: " + commentRevision.NewLength);
                }
            }

            // Salva la cartella di lavoro con le revisioni
            workbook.Save("RevisionCellCommentPropertyActionTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


