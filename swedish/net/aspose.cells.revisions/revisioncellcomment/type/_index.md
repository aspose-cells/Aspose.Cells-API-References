---
title: "RevisionCellComment.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionCellComment‑egenskapen. Hämtar revisionstypen"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncellcomment/type/
---
## RevisionCellComment.Type property

Hämtar typen av revision.

```csharp
public override RevisionType Type { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar till cell A1
            int commentRow = 0;
            int commentCol = 0;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Initial comment";

            // Spåra revisioner – ändrad till att använda HasRevisions‑egenskapen
            // Obs: Vid faktisk användning kan du behöva aktivera spårning på annat sätt
            // eftersom HasRevisions är en skrivskyddad egenskap som indikerar om revisioner finns

            // Ändra kommentaren för att skapa en revision
            comment.Note = "Modified comment";

            // Kom åt revisionerna via Workbook:s RevisionLogs‑samling
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Visa värdet för Type-egenskapen
                    Console.WriteLine("Revision Type: " + commentRevision.Type);
                    
                    // Demonstrera användning av Type‑egenskapen
                    if (commentRevision.Type == RevisionType.Comment)
                    {
                        Console.WriteLine("This revision is related to a comment change");
                        Console.WriteLine("Comment was modified at row: " + commentRevision.Row + ", column: " + commentRevision.Column);
                        Console.WriteLine("Old comment length: " + commentRevision.OldLength);
                        Console.WriteLine("New comment length: " + commentRevision.NewLength);
                    }
                }
            }

            // Spara arbetsboken med revisioner
            workbook.Save("RevisionCellCommentPropertyTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [RevisionType](../../revisiontype/)
* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


