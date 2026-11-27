---
title: "RevisionCellComment.ActionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionCellComment‑egenskapen. Hämtar åtgärdstypen för revisionen"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncellcomment/actiontype/
---
## RevisionCellComment.ActionType property

Hämtar åtgärdstypen för revisionen.

```csharp
public RevisionActionType ActionType { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok med revisionsspårning
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar till cell A1
            Comment comment = worksheet.Comments[0, 0];
            comment.Note = "Initial comment";

            // Ändra kommentaren för att skapa en revision
            comment.Note = "Updated comment";

            // Lägg till en ny kommentar för att generera en Add‑revision
            Comment newComment = worksheet.Comments[1, 1];
            newComment.Note = "New comment";

            // Åtkomst till revisionerna
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Visa ActionType‑egenskapens värde
                    Console.WriteLine("Revision ActionType: " + commentRevision.ActionType);
                    
                    // Demonstrera användning av egenskapen ActionType
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

                    // Visa relaterade egenskaper
                    Console.WriteLine("Comment location: " + commentRevision.CellName);
                    Console.WriteLine("Is old comment: " + commentRevision.IsOldComment);
                    Console.WriteLine("Old length: " + commentRevision.OldLength);
                    Console.WriteLine("New length: " + commentRevision.NewLength);
                }
            }

            // Spara arbetsboken med revisioner
            workbook.Save("RevisionCellCommentPropertyActionTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


