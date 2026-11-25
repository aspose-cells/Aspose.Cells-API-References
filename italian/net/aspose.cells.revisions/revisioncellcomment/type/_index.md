---
title: "RevisionCellComment.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionCellComment. Restituisce il tipo di revisione"
type: docs
url: /it/net/aspose.cells.revisions/revisioncellcomment/type/
---
## RevisionCellComment.Type property

Ottiene il tipo di revisione.

```csharp
public override RevisionType Type { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento alla cella A1
            int commentRow = 0;
            int commentCol = 0;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Initial comment";

            // Traccia le revisioni - modificato per utilizzare la proprietà HasRevisions
            // Nota: Nell'uso reale, potresti dover abilitare il tracciamento tramite altri metodi
            // poiché HasRevisions è una proprietà di sola lettura che indica se esistono revisioni

            // Modifica il commento per generare una revisione
            comment.Note = "Modified comment";

            // Accedi alle revisioni tramite la collezione RevisionLogs del Workbook
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Visualizza il valore della proprietà Type
                    Console.WriteLine("Revision Type: " + commentRevision.Type);
                    
                    // Dimostra l'uso della proprietà Type
                    if (commentRevision.Type == RevisionType.Comment)
                    {
                        Console.WriteLine("This revision is related to a comment change");
                        Console.WriteLine("Comment was modified at row: " + commentRevision.Row + ", column: " + commentRevision.Column);
                        Console.WriteLine("Old comment length: " + commentRevision.OldLength);
                        Console.WriteLine("New comment length: " + commentRevision.NewLength);
                    }
                }
            }

            // Salva la cartella di lavoro con le revisioni
            workbook.Save("RevisionCellCommentPropertyTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [RevisionType](../../revisiontype/)
* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


