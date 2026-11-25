---
title: "RevisionCellComment.CellName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionCellComment. Ottiene il nome della cella"
type: docs
url: /it/net/aspose.cells.revisions/revisioncellcomment/cellname/
---
## RevisionCellComment.CellName property

Ottiene il nome della cella.

```csharp
public string CellName { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyCellNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento alla cella B5
            int commentRow = 4;
            int commentCol = 1;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Initial comment";

            // Modifica il commento per generare una revisione
            comment.Note = "Updated comment";

            // Accedi alle revisioni
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Visualizza il valore corrente di CellName
                    Console.WriteLine("Original CellName: " + commentRevision.CellName);
                    
                    // Modifica la proprietà CellName
                    commentRevision.CellName = "C10";
                    Console.WriteLine("Modified CellName: " + commentRevision.CellName);
                    
                    // Dimostra l'effetto della modifica di CellName
                    Console.WriteLine("Row index: " + commentRevision.Row);
                    Console.WriteLine("Column index: " + commentRevision.Column);
                    
                    // Nota: Modificando CellName si aggiornano le proprietà Row/Column
                    Console.WriteLine("After CellName change - Row: " + commentRevision.Row);
                    Console.WriteLine("After CellName change - Column: " + commentRevision.Column);
                }
            }

            // Salva la cartella di lavoro con le revisioni
            workbook.Save("RevisionCellCommentPropertyCellNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


