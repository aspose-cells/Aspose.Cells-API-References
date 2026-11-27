---
title: "RevisionCellComment.OldLength"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionCellComment-egenskap. Hämtar längden på kommentartexten som lagts till i denna revision"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncellcomment/oldlength/
---
## RevisionCellComment.OldLength property

Hämtar längden på kommentartexten som lades till i denna revision.

```csharp
public int OldLength { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok med revisionsspårning
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar till cell D4
            int commentRow = 3;
            int commentCol = 3;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            string initialComment = "Original comment text";
            comment.Note = initialComment;

            // Ändra kommentaren för att skapa en revision
            string updatedComment = "This is the modified comment text with more content";
            comment.Note = updatedComment;

            // Åtkomst till revisionerna
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Visa värdet för egenskapen OldLength
                    Console.WriteLine("Old comment length: " + commentRevision.OldLength);
                    Console.WriteLine("Actual initial comment length: " + initialComment.Length);
                    
                    // Visa relaterade egenskaper
                    Console.WriteLine("New comment length: " + commentRevision.NewLength);
                    Console.WriteLine("Comment location: " + commentRevision.CellName);
                    
                    // Demonstrera användning av egenskapen OldLength
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

            // Spara arbetsboken med revisioner
            workbook.Save("RevisionCellCommentPropertyOldLengthDemo.xlsx");
        }
    }
}
```

### Se även

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


