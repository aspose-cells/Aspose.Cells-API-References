---
title: "Klass RevisionCellComment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Revisions.RevisionCellComment-klass. Representerar en revisionspost för en ändring av en cellkommentar"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncellcomment/
---
## RevisionCellComment class

Representerar en revisionspost för en ändring av en cellkommentar.

```csharp
public class RevisionCellComment : Revision
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioncellcomment/actiontype/) { get; } | Hämtar åtgärdstypen för revisionen. |
| [CellName](../../aspose.cells.revisions/revisioncellcomment/cellname/) { get; set; } | Hämtar cellens namn. |
| [Column](../../aspose.cells.revisions/revisioncellcomment/column/) { get; } | Hämtar kolumnindex för den som innehåller en kommentar. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Hämtar numret för denna revision.(Arv från [`Revision`](../revision/).) |
| [IsOldComment](../../aspose.cells.revisions/revisioncellcomment/isoldcomment/) { get; } | Indikerar om det är en gammal kommentar. |
| [NewLength](../../aspose.cells.revisions/revisioncellcomment/newlength/) { get; } | Hämtar längden på kommentaren innan denna revision gjordes. |
| [OldLength](../../aspose.cells.revisions/revisioncellcomment/oldlength/) { get; } | Hämtar längden på kommentartexten som lades till i denna revision. |
| [Row](../../aspose.cells.revisions/revisioncellcomment/row/) { get; } | Hämtar radindex för den som innehåller en kommentar. |
| override [Type](../../aspose.cells.revisions/revisioncellcomment/type/) { get; } | Hämtar typen av revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Hämtar kalkylbladet.(Arv från [`Revision`](../revision/).) |

### Exempel

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
            // Skapa en ny arbetsbok med revisionsspårning
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till initial kommentar till cell A1
            Comment comment = worksheet.Comments[0, 0];
            comment.Note = "Initial comment text";

            // Ändra kommentaren för att skapa en revision
            comment.Note = "Updated comment with more text";

            // Kom åt revisionsloggen
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;

                    // Visa revisionsegenskaper
                    Console.WriteLine("Revision Type: " + commentRevision.Type);
                    Console.WriteLine("Action Type: " + commentRevision.ActionType);
                    Console.WriteLine("Cell Location: " + commentRevision.CellName);
                    Console.WriteLine("Row: " + commentRevision.Row);
                    Console.WriteLine("Column: " + commentRevision.Column);

                    // Visa förändringar i kommentarslängd
                    Console.WriteLine("Old Length: " + commentRevision.OldLength);
                    Console.WriteLine("New Length: " + commentRevision.NewLength);
                    Console.WriteLine("Is Old Comment: " + commentRevision.IsOldComment);

                    // Ändra cellnamn för att demonstrera egenskapsändring
                    string originalCellName = commentRevision.CellName;
                    commentRevision.CellName = "B2";
                    Console.WriteLine("Modified Cell Location: " + commentRevision.CellName);
                    Console.WriteLine("New Row: " + commentRevision.Row);
                    Console.WriteLine("New Column: " + commentRevision.Column);

                    // Återställ originalcellnamnet
                    commentRevision.CellName = originalCellName;
                }
            }

            // Spara arbetsboken med revisioner
            workbook.Save("RevisionsClassRevisionCellCommentDemo.xlsx");
        }
    }
}
```

### Se även

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


