---
title: "RevisionCellComment.OldLength"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionCellComment. Restituisce la lunghezza del testo del commento aggiunto in questa revisione"
type: docs
url: /it/net/aspose.cells.revisions/revisioncellcomment/oldlength/
---
## RevisionCellComment.OldLength property

Ottiene la lunghezza del testo del commento aggiunto in questa revisione.

```csharp
public int OldLength { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyOldLengthDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con tracciamento delle revisioni
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento alla cella D4
            int commentRow = 3;
            int commentCol = 3;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            string initialComment = "Original comment text";
            comment.Note = initialComment;

            // Modifica il commento per generare una revisione
            string updatedComment = "This is the modified comment text with more content";
            comment.Note = updatedComment;

            // Accedi alle revisioni
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Visualizza il valore della proprietà OldLength
                    Console.WriteLine("Old comment length: " + commentRevision.OldLength);
                    Console.WriteLine("Actual initial comment length: " + initialComment.Length);
                    
                    // Visualizza le proprietà correlate
                    Console.WriteLine("New comment length: " + commentRevision.NewLength);
                    Console.WriteLine("Comment location: " + commentRevision.CellName);
                    
                    // Dimostra l'uso della proprietà OldLength
                    if (commentRevision.OldLength > 0)
                    {
                        Console.WriteLine("Comment existed before modification with length: " + 
                            commentRevision.OldLength);
                            
                        double expansionPercentage = ((double)(commentRevision.NewLength - commentRevision.OldLength) / 
                            commentRevision.OldLength) * 100;
                        Console.WriteLine($"Comment expanded by {expansionPercentage:F2}%");
                    }
                }
            }

            // Salva la cartella di lavoro con le revisioni
            workbook.Save("RevisionCellCommentPropertyOldLengthDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


