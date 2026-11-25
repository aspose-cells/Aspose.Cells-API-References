---
title: "RevisionCellComment.Row"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionCellComment. Restituisce l'indice di riga di quello che contiene un commento"
type: docs
url: /it/net/aspose.cells.revisions/revisioncellcomment/row/
---
## RevisionCellComment.Row property

Ottiene l'indice della riga della cella che contiene un commento.

```csharp
public int Row { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con tracciamento delle revisioni
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento alla cella D4 (riga 3, colonna 3)
            int commentRow = 3;
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
                    
                    // Visualizza il valore della proprietà Row
                    Console.WriteLine("Comment is located at row: " + commentRevision.Row);
                    
                    // Dimostra l'uso della proprietà Row
                    Console.WriteLine("Comment location details:");
                    Console.WriteLine("Row index: " + commentRevision.Row);
                    Console.WriteLine("Column index: " + commentRevision.Column);
                    Console.WriteLine("Cell name: " + commentRevision.CellName);
                    
                    // Mostra che Row è sola lettura tentando di modificarla (causerà un errore di compilazione)
                    // commentRevision.Row = 5; // Questa riga è commentata perché Row è sola lettura
                    
                    // Metodo alternativo per cambiare la posizione modificando CellName
                    Console.WriteLine("\nChanging comment position via CellName...");
                    commentRevision.CellName = "F10"; // Changes to row 9, column 5
                    Console.WriteLine("New Row index: " + commentRevision.Row);
                    Console.WriteLine("New Column index: " + commentRevision.Column);
                }
            }

            // Salva la cartella di lavoro con le revisioni
            workbook.Save("RevisionCellCommentPropertyRowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


