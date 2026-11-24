---
title: "RevisionCellComment.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionCellComment-Eigenschaft. Gibt den Typ der Revision zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisioncellcomment/type/
---
## RevisionCellComment.Type property

Liest den Typ der Revision.

```csharp
public override RevisionType Type { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einen Kommentar zur Zelle A1 hinzufügen
            int commentRow = 0;
            int commentCol = 0;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Initial comment";

            // Revisionen verfolgen – geändert, um die HasRevisions-Eigenschaft zu verwenden
            // Hinweis: In der tatsächlichen Verwendung müssen Sie möglicherweise die Verfolgung auf andere Weise aktivieren
            // da HasRevisions eine schreibgeschützte Eigenschaft ist, die anzeigt, ob Revisionen existieren

            // Ändern Sie den Kommentar, um eine Revision zu erstellen
            comment.Note = "Modified comment";

            // Greifen Sie auf die Revisionen über die RevisionLogs-Sammlung des Workbook zu
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Den Wert der Type-Eigenschaft anzeigen
                    Console.WriteLine("Revision Type: " + commentRevision.Type);
                    
                    // Demonstrieren Sie die Verwendung der Type-Eigenschaft
                    if (commentRevision.Type == RevisionType.Comment)
                    {
                        Console.WriteLine("This revision is related to a comment change");
                        Console.WriteLine("Comment was modified at row: " + commentRevision.Row + ", column: " + commentRevision.Column);
                        Console.WriteLine("Old comment length: " + commentRevision.OldLength);
                        Console.WriteLine("New comment length: " + commentRevision.NewLength);
                    }
                }
            }

            // Speichern Sie die Arbeitsmappe mit Revisionen
            workbook.Save("RevisionCellCommentPropertyTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [RevisionType](../../revisiontype/)
* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


