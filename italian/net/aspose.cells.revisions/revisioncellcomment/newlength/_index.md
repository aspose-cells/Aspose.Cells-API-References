---
title: "RevisionCellComment.NewLength"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionCellComment. Ottiene la lunghezza del commento prima che questa revisione fosse effettuata"
type: docs
url: /it/net/aspose.cells.revisions/revisioncellcomment/newlength/
---
## RevisionCellComment.NewLength property

Ottiene la lunghezza del commento prima che questa revisione fosse effettuata.

```csharp
public int NewLength { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyNewLengthDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con tracciamento delle revisioni
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento alla cella F7
            int commentRow = 6;
            int commentCol = 5;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Initial comment text";

            // Modifica il commento per generare una revisione
            string updatedComment = "This is an updated and longer comment text";
            comment.Note = updatedComment;

            // Accedi alle revisioni
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Visualizza il valore della proprietà NewLength
                    Console.WriteLine("New comment length: " + commentRevision.NewLength);
                    Console.WriteLine("Actual new comment length: " + updatedComment.Length);
                    
                    // Visualizza le proprietà correlate
                    Console.WriteLine("Old comment length: " + commentRevision.OldLength);
                    Console.WriteLine("Comment location: " + commentRevision.CellName);
                    
                    // Dimostra l'uso della proprietà NewLength
                    if (commentRevision.NewLength > commentRevision.OldLength)
                    {
                        Console.WriteLine("Comment was expanded by " + 
                            (commentRevision.NewLength - commentRevision.OldLength) + " characters");
                    }
                    else if (commentRevision.NewLength < commentRevision.OldLength)
                    {
                        Console.WriteLine("Comment was shortened by " + 
                            (commentRevision.OldLength - commentRevision.NewLength) + " characters");
                    }
                    else
                    {
                        Console.WriteLine("Comment length remained the same");
                    }
                }
            }

            // Salva la cartella di lavoro con le revisioni
            workbook.Save("RevisionCellCommentPropertyNewLengthDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


