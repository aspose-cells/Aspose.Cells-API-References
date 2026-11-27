---
title: "RevisionCellComment.Column"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionCellComment‑egenskapen. Hämtar kolumnindexet för den som innehåller en kommentar"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncellcomment/column/
---
## RevisionCellComment.Column property

Hämtar kolumnindex för den som innehåller en kommentar.

```csharp
public int Column { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar till cell D3
            int commentRow = 2;
            int commentCol = 3;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Sample comment for revision tracking";

            // Ändra kommentaren för att skapa en revision
            comment.Note = "Updated comment text";

            // Åtkomst till revisionerna
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Visa Column‑egenskapens värde
                    Console.WriteLine("Comment revision column index: " + commentRevision.Column);
                    
                    // Demonstrera användning av Column‑egenskapen
                    Console.WriteLine("Comment was modified in column: " + (char)('A' + commentRevision.Column));
                    
                    // Visa relaterade egenskaper
                    Console.WriteLine("Associated row: " + commentRevision.Row);
                    Console.WriteLine("Cell name: " + commentRevision.CellName);
                    
                    // Obs: Column är skrivskyddad, så vi kan inte ändra den direkt
                    // Vi kan ändra den indirekt genom att modifiera CellName
                    string originalCellName = commentRevision.CellName;
                    commentRevision.CellName = "E5"; // This will update both Row and Column properties
                    Console.WriteLine("After CellName change - New column: " + commentRevision.Column);
                    
                    // Återställ originalvärdet
                    commentRevision.CellName = originalCellName;
                }
            }

            // Spara arbetsboken med revisioner
            workbook.Save("RevisionCellCommentPropertyColumnDemo.xlsx");
        }
    }
}
```

### Se även

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


