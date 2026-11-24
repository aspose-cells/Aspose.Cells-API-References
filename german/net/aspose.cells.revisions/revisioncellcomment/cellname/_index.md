---
title: "RevisionCellComment.CellName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionCellComment-Eigenschaft. Gibt den Namen der Zelle zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisioncellcomment/cellname/
---
## RevisionCellComment.CellName property

Ermittelt den Namen der Zelle.

```csharp
public string CellName { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einen Kommentar zur Zelle B5 hinzu
            int commentRow = 4;
            int commentCol = 1;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Initial comment";

            // Ändern Sie den Kommentar, um eine Revision zu erstellen
            comment.Note = "Updated comment";

            // Zugriff auf die Revisionen
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Zeige den aktuellen Wert von CellName an
                    Console.WriteLine("Original CellName: " + commentRevision.CellName);
                    
                    // Ändern Sie die CellName-Eigenschaft
                    commentRevision.CellName = "C10";
                    Console.WriteLine("Modified CellName: " + commentRevision.CellName);
                    
                    // Demonstrieren Sie die Auswirkung der Änderung von CellName
                    Console.WriteLine("Row index: " + commentRevision.Row);
                    Console.WriteLine("Column index: " + commentRevision.Column);
                    
                    // Hinweis: Das Ändern von CellName aktualisiert die Row/Column-Eigenschaften
                    Console.WriteLine("After CellName change - Row: " + commentRevision.Row);
                    Console.WriteLine("After CellName change - Column: " + commentRevision.Column);
                }
            }

            // Speichern Sie die Arbeitsmappe mit Revisionen
            workbook.Save("RevisionCellCommentPropertyCellNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


