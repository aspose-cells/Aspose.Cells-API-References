---
title: "RevisionCellComment.Row"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionCellComment-Eigenschaft. Gibt den Zeilenindex zurück, der einen Kommentar enthält"
type: docs
url: /de/net/aspose.cells.revisions/revisioncellcomment/row/
---
## RevisionCellComment.Row property

Gibt den Zeilenindex zurück, der einen Kommentar enthält.

```csharp
public int Row { get; }
```

### Beispiele

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
            // Erstelle eine neue Arbeitsmappe mit Revisionsverfolgung
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einen Kommentar zur Zelle D4 (Zeile 3, Spalte 3) hinzu
            int commentRow = 3;
            int commentCol = 3;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Sample comment for revision tracking";

            // Ändern Sie den Kommentar, um eine Revision zu erstellen
            comment.Note = "Updated comment text";

            // Zugriff auf die Revisionen
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Anzeige des Row-Eigenschaftswerts
                    Console.WriteLine("Comment is located at row: " + commentRevision.Row);
                    
                    // Demonstriere die Verwendung der Row-Eigenschaft
                    Console.WriteLine("Comment location details:");
                    Console.WriteLine("Row index: " + commentRevision.Row);
                    Console.WriteLine("Column index: " + commentRevision.Column);
                    Console.WriteLine("Cell name: " + commentRevision.CellName);
                    
                    // Zeige, dass Row schreibgeschützt ist, indem versucht wird, sie zu ändern (führt zu einem Kompilierungsfehler)
                    // commentRevision.Row = 5; // Diese Zeile ist auskommentiert, da Row schreibgeschützt ist
                    
                    // Alternative Möglichkeit, die Position zu ändern, indem CellName modifiziert wird
                    Console.WriteLine("\nChanging comment position via CellName...");
                    commentRevision.CellName = "F10"; // Changes to row 9, column 5
                    Console.WriteLine("New Row index: " + commentRevision.Row);
                    Console.WriteLine("New Column index: " + commentRevision.Column);
                }
            }

            // Speichern Sie die Arbeitsmappe mit Revisionen
            workbook.Save("RevisionCellCommentPropertyRowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


