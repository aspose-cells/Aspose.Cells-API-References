---
title: "RevisionCellComment.NewLength"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionCellComment-egenskap. Hämtar längden på kommentaren innan denna revision gjordes"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncellcomment/newlength/
---
## RevisionCellComment.NewLength property

Hämtar längden på kommentaren innan denna revision gjordes.

```csharp
public int NewLength { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok med revisionsspårning
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar till cell F7
            int commentRow = 6;
            int commentCol = 5;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Initial comment text";

            // Ändra kommentaren för att skapa en revision
            string updatedComment = "This is an updated and longer comment text";
            comment.Note = updatedComment;

            // Åtkomst till revisionerna
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Visa värdet för egenskapen NewLength
                    Console.WriteLine("New comment length: " + commentRevision.NewLength);
                    Console.WriteLine("Actual new comment length: " + updatedComment.Length);
                    
                    // Visa relaterade egenskaper
                    Console.WriteLine("Old comment length: " + commentRevision.OldLength);
                    Console.WriteLine("Comment location: " + commentRevision.CellName);
                    
                    // Demonstrera användning av egenskapen NewLength
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

            // Spara arbetsboken med revisioner
            workbook.Save("RevisionCellCommentPropertyNewLengthDemo.xlsx");
        }
    }
}
```

### Se även

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


