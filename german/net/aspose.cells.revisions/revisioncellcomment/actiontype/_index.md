---
title: "RevisionCellComment.ActionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionCellComment-Eigenschaft. Gibt den Aktionstyp der Revision zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisioncellcomment/actiontype/
---
## RevisionCellComment.ActionType property

Liest den Aktionstyp der Revision.

```csharp
public RevisionActionType ActionType { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyActionTypeDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe mit Revisionsverfolgung
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einen Kommentar zur Zelle A1 hinzufügen
            Comment comment = worksheet.Comments[0, 0];
            comment.Note = "Initial comment";

            // Ändern Sie den Kommentar, um eine Revision zu erstellen
            comment.Note = "Updated comment";

            // Fügen Sie einen neuen Kommentar hinzu, um eine Add revision zu erzeugen
            Comment newComment = worksheet.Comments[1, 1];
            newComment.Note = "New comment";

            // Zugriff auf die Revisionen
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Zeigen Sie den Wert der ActionType-Eigenschaft an
                    Console.WriteLine("Revision ActionType: " + commentRevision.ActionType);
                    
                    // Demonstrieren Sie die Verwendung der ActionType-Eigenschaft
                    switch (commentRevision.ActionType)
                    {
                        case RevisionActionType.Add:
                            Console.WriteLine("This revision added a new comment at " + commentRevision.CellName);
                            break;
                        case RevisionActionType.Delete:
                            Console.WriteLine("This revision deleted a comment from " + commentRevision.CellName);
                            break;
                        default:
                            Console.WriteLine("This revision modified a comment at " + commentRevision.CellName);
                            break;
                    }

                    // Zeige verwandte Eigenschaften an
                    Console.WriteLine("Comment location: " + commentRevision.CellName);
                    Console.WriteLine("Is old comment: " + commentRevision.IsOldComment);
                    Console.WriteLine("Old length: " + commentRevision.OldLength);
                    Console.WriteLine("New length: " + commentRevision.NewLength);
                }
            }

            // Speichern Sie die Arbeitsmappe mit Revisionen
            workbook.Save("RevisionCellCommentPropertyActionTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


