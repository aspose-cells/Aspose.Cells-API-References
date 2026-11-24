---
title: "RevisionCellComment.Column"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionCellComment-Eigenschaft. Gibt den Spaltenindex zurück, der einen Kommentar enthält"
type: docs
url: /de/net/aspose.cells.revisions/revisioncellcomment/column/
---
## RevisionCellComment.Column property

Gibt den Spaltenindex zurück, der einen Kommentar enthält.

```csharp
public int Column { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einen Kommentar zu Zelle D3 hinzu
            int commentRow = 2;
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
                    
                    // Zeigen Sie den Wert der Column-Eigenschaft an
                    Console.WriteLine("Comment revision column index: " + commentRevision.Column);
                    
                    // Demonstrieren Sie die Verwendung der Column-Eigenschaft
                    Console.WriteLine("Comment was modified in column: " + (char)('A' + commentRevision.Column));
                    
                    // Zeige verwandte Eigenschaften an
                    Console.WriteLine("Associated row: " + commentRevision.Row);
                    Console.WriteLine("Cell name: " + commentRevision.CellName);
                    
                    // Hinweis: Column ist schreibgeschützt, daher können wir es nicht direkt ändern
                    // Wir können es indirekt ändern, indem wir CellName modifizieren
                    string originalCellName = commentRevision.CellName;
                    commentRevision.CellName = "E5"; // This will update both Row and Column properties
                    Console.WriteLine("After CellName change - New column: " + commentRevision.Column);
                    
                    // Ursprünglichen Wert wiederherstellen
                    commentRevision.CellName = originalCellName;
                }
            }

            // Speichern Sie die Arbeitsmappe mit Revisionen
            workbook.Save("RevisionCellCommentPropertyColumnDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


