---
title: "Classe RevisionCellComment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Revisions.RevisionCellComment. Rappresenta un record di revisione di una modifica al commento di una cella"
type: docs
url: /it/net/aspose.cells.revisions/revisioncellcomment/
---
## RevisionCellComment class

Rappresenta un record di revisione di una modifica al commento di una cella.

```csharp
public class RevisionCellComment : Revision
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioncellcomment/actiontype/) { get; } | Ottiene il tipo di azione della revisione. |
| [CellName](../../aspose.cells.revisions/revisioncellcomment/cellname/) { get; set; } | Ottiene il nome della cella. |
| [Column](../../aspose.cells.revisions/revisioncellcomment/column/) { get; } | Ottiene l'indice della colonna della cella che contiene un commento. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Ottiene il numero di questa revisione.(Ereditato da [`Revision`](../revision/).) |
| [IsOldComment](../../aspose.cells.revisions/revisioncellcomment/isoldcomment/) { get; } | Indica se è un commento precedente. |
| [NewLength](../../aspose.cells.revisions/revisioncellcomment/newlength/) { get; } | Ottiene la lunghezza del commento prima che questa revisione fosse effettuata. |
| [OldLength](../../aspose.cells.revisions/revisioncellcomment/oldlength/) { get; } | Ottiene la lunghezza del testo del commento aggiunto in questa revisione. |
| [Row](../../aspose.cells.revisions/revisioncellcomment/row/) { get; } | Ottiene l'indice della riga della cella che contiene un commento. |
| override [Type](../../aspose.cells.revisions/revisioncellcomment/type/) { get; } | Ottiene il tipo di revisione. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Ottiene il foglio di lavoro.(Ereditato da [`Revision`](../revision/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionCellCommentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con tracciamento delle revisioni
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi il commento iniziale alla cella A1
            Comment comment = worksheet.Comments[0, 0];
            comment.Note = "Initial comment text";

            // Modifica il commento per generare una revisione
            comment.Note = "Updated comment with more text";

            // Accedi al registro delle revisioni
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;

                    // Visualizza le proprietà della revisione
                    Console.WriteLine("Revision Type: " + commentRevision.Type);
                    Console.WriteLine("Action Type: " + commentRevision.ActionType);
                    Console.WriteLine("Cell Location: " + commentRevision.CellName);
                    Console.WriteLine("Row: " + commentRevision.Row);
                    Console.WriteLine("Column: " + commentRevision.Column);

                    // Mostra le variazioni di lunghezza del commento
                    Console.WriteLine("Old Length: " + commentRevision.OldLength);
                    Console.WriteLine("New Length: " + commentRevision.NewLength);
                    Console.WriteLine("Is Old Comment: " + commentRevision.IsOldComment);

                    // Modifica il nome della cella per dimostrare il cambiamento della proprietà
                    string originalCellName = commentRevision.CellName;
                    commentRevision.CellName = "B2";
                    Console.WriteLine("Modified Cell Location: " + commentRevision.CellName);
                    Console.WriteLine("New Row: " + commentRevision.Row);
                    Console.WriteLine("New Column: " + commentRevision.Column);

                    // Ripristina il nome originale della cella
                    commentRevision.CellName = originalCellName;
                }
            }

            // Salva la cartella di lavoro con le revisioni
            workbook.Save("RevisionsClassRevisionCellCommentDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


