---
title: "RevisionCellComment.CellName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionCellComment‑egenskapen. Hämtar namnet på cellen"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncellcomment/cellname/
---
## RevisionCellComment.CellName property

Hämtar cellens namn.

```csharp
public string CellName { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar till cell B5
            int commentRow = 4;
            int commentCol = 1;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Initial comment";

            // Ändra kommentaren för att skapa en revision
            comment.Note = "Updated comment";

            // Åtkomst till revisionerna
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Visa aktuellt CellName‑värde
                    Console.WriteLine("Original CellName: " + commentRevision.CellName);
                    
                    // Ändra CellName‑egenskapen
                    commentRevision.CellName = "C10";
                    Console.WriteLine("Modified CellName: " + commentRevision.CellName);
                    
                    // Demonstrera effekten av att ändra CellName
                    Console.WriteLine("Row index: " + commentRevision.Row);
                    Console.WriteLine("Column index: " + commentRevision.Column);
                    
                    // Obs: Att ändra CellName uppdaterar Row/Column‑egenskaperna
                    Console.WriteLine("After CellName change - Row: " + commentRevision.Row);
                    Console.WriteLine("After CellName change - Column: " + commentRevision.Column);
                }
            }

            // Spara arbetsboken med revisioner
            workbook.Save("RevisionCellCommentPropertyCellNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


