---
title: "RevisionCellComment.Row"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionCellComment egenskap. Hämtar radindex för den som innehåller en kommentar"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncellcomment/row/
---
## RevisionCellComment.Row property

Hämtar radindex för den som innehåller en kommentar.

```csharp
public int Row { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok med revisionsspårning
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar till cell D4 (rad 3, kolumn 3)
            int commentRow = 3;
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
                    
                    // Visa värdet för egenskapen Row
                    Console.WriteLine("Comment is located at row: " + commentRevision.Row);
                    
                    // Demonstrera användning av egenskapen Row
                    Console.WriteLine("Comment location details:");
                    Console.WriteLine("Row index: " + commentRevision.Row);
                    Console.WriteLine("Column index: " + commentRevision.Column);
                    Console.WriteLine("Cell name: " + commentRevision.CellName);
                    
                    // Visa att Row är skrivskyddad genom att försöka ändra den (kommer att orsaka kompileringsfel)
                    // commentRevision.Row = 5; // Den här raden är kommenterad eftersom Row är skrivskyddad
                    
                    // Alternativt sätt att ändra position genom att modifiera CellName
                    Console.WriteLine("\nChanging comment position via CellName...");
                    commentRevision.CellName = "F10"; // Changes to row 9, column 5
                    Console.WriteLine("New Row index: " + commentRevision.Row);
                    Console.WriteLine("New Column index: " + commentRevision.Column);
                }
            }

            // Spara arbetsboken med revisioner
            workbook.Save("RevisionCellCommentPropertyRowDemo.xlsx");
        }
    }
}
```

### Se även

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


