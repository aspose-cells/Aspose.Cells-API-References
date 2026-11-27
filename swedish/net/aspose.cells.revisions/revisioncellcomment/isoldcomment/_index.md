---
title: "RevisionCellComment.IsOldComment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionCellComment-egenskap. Anger om det är en gammal kommentar"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncellcomment/isoldcomment/
---
## RevisionCellComment.IsOldComment property

Indikerar om det är en gammal kommentar.

```csharp
public bool IsOldComment { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyIsOldCommentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med revisionsspårning
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till initial kommentar till cell A1
            Comment comment = worksheet.Comments[0, 0];
            comment.Note = "First version of comment";

            // Ändra kommentaren för att skapa en revision
            comment.Note = "Updated comment text";

            // Lägg till en annan kommentar till cell B2
            Comment secondComment = worksheet.Comments[1, 1];
            secondComment.Note = "Second comment";

            // Åtkomst till revisionerna
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Visa värdet för egenskapen IsOldComment
                    Console.WriteLine("Cell: " + commentRevision.CellName);
                    Console.WriteLine("IsOldComment: " + commentRevision.IsOldComment);
                    
                    // Demonstrera användning av egenskapen IsOldComment
                    if (commentRevision.IsOldComment)
                    {
                        Console.WriteLine("This revision represents the old state of the comment");
                        Console.WriteLine("Old comment length: " + commentRevision.OldLength);
                    }
                    else
                    {
                        Console.WriteLine("This revision represents the new state of the comment");
                        Console.WriteLine("New comment length: " + commentRevision.NewLength);
                    }

                    // Visa relaterade egenskaper
                    Console.WriteLine("Action Type: " + commentRevision.ActionType);
                    Console.WriteLine("Revision Type: " + commentRevision.Type);
                }
            }

            // Spara arbetsboken med revisioner
            workbook.Save("RevisionCellCommentPropertyIsOldCommentDemo.xlsx");
        }
    }
}
```

### Se även

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


