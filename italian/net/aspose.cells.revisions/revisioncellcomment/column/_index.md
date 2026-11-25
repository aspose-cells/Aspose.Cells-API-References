---
title: "RevisionCellComment.Column"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionCellComment. Ottiene l'indice di colonna di quello che contiene un commento"
type: docs
url: /it/net/aspose.cells.revisions/revisioncellcomment/column/
---
## RevisionCellComment.Column property

Ottiene l'indice della colonna della cella che contiene un commento.

```csharp
public int Column { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento alla cella D3
            int commentRow = 2;
            int commentCol = 3;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Sample comment for revision tracking";

            // Modifica il commento per generare una revisione
            comment.Note = "Updated comment text";

            // Accedi alle revisioni
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Visualizza il valore della proprietà Column
                    Console.WriteLine("Comment revision column index: " + commentRevision.Column);
                    
                    // Dimostra l'uso della proprietà Column
                    Console.WriteLine("Comment was modified in column: " + (char)('A' + commentRevision.Column));
                    
                    // Mostra le proprietà correlate
                    Console.WriteLine("Associated row: " + commentRevision.Row);
                    Console.WriteLine("Cell name: " + commentRevision.CellName);
                    
                    // Nota: Column è di sola lettura, quindi non possiamo modificarla direttamente
                    // Possiamo cambiarla indirettamente modificando CellName
                    string originalCellName = commentRevision.CellName;
                    commentRevision.CellName = "E5"; // This will update both Row and Column properties
                    Console.WriteLine("After CellName change - New column: " + commentRevision.Column);
                    
                    // Ripristina il valore originale
                    commentRevision.CellName = originalCellName;
                }
            }

            // Salva la cartella di lavoro con le revisioni
            workbook.Save("RevisionCellCommentPropertyColumnDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


