---
title: "Klasse RevisionCellComment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Revisions.RevisionCellComment Klasse. Stellt einen Revisionsdatensatz einer Zellkommentaränderung dar"
type: docs
url: /de/net/aspose.cells.revisions/revisioncellcomment/
---
## RevisionCellComment class

Stellt einen Revisionsdatensatz einer Zellkommentaränderung dar.

```csharp
public class RevisionCellComment : Revision
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioncellcomment/actiontype/) { get; } | Liest den Aktionstyp der Revision. |
| [CellName](../../aspose.cells.revisions/revisioncellcomment/cellname/) { get; set; } | Ermittelt den Namen der Zelle. |
| [Column](../../aspose.cells.revisions/revisioncellcomment/column/) { get; } | Gibt den Spaltenindex zurück, der einen Kommentar enthält. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Ermittelt die Nummer dieser Revision.(Vererbt von [`Revision`](../revision/).) |
| [IsOldComment](../../aspose.cells.revisions/revisioncellcomment/isoldcomment/) { get; } | Gibt an, ob es ein alter Kommentar ist. |
| [NewLength](../../aspose.cells.revisions/revisioncellcomment/newlength/) { get; } | Gibt die Länge des Kommentars vor dieser Revision zurück. |
| [OldLength](../../aspose.cells.revisions/revisioncellcomment/oldlength/) { get; } | Gibt die Länge des in dieser Revision hinzugefügten Kommentartexts zurück. |
| [Row](../../aspose.cells.revisions/revisioncellcomment/row/) { get; } | Gibt den Zeilenindex zurück, der einen Kommentar enthält. |
| override [Type](../../aspose.cells.revisions/revisioncellcomment/type/) { get; } | Liest den Typ der Revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Ermittelt das Arbeitsblatt.(Vererbt von [`Revision`](../revision/).) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionCellCommentDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe mit Revisionsverfolgung
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einen Anfangskommentar zur Zelle A1 hinzu
            Comment comment = worksheet.Comments[0, 0];
            comment.Note = "Initial comment text";

            // Ändern Sie den Kommentar, um eine Revision zu erstellen
            comment.Note = "Updated comment with more text";

            // Greifen Sie auf das Revisionsprotokoll zu
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;

                    // Revisions‑Eigenschaften anzeigen
                    Console.WriteLine("Revision Type: " + commentRevision.Type);
                    Console.WriteLine("Action Type: " + commentRevision.ActionType);
                    Console.WriteLine("Cell Location: " + commentRevision.CellName);
                    Console.WriteLine("Row: " + commentRevision.Row);
                    Console.WriteLine("Column: " + commentRevision.Column);

                    // Änderungen der Kommentarlänge anzeigen
                    Console.WriteLine("Old Length: " + commentRevision.OldLength);
                    Console.WriteLine("New Length: " + commentRevision.NewLength);
                    Console.WriteLine("Is Old Comment: " + commentRevision.IsOldComment);

                    // Ändern Sie den Zellenamen, um die Eigenschaftsänderung zu demonstrieren
                    string originalCellName = commentRevision.CellName;
                    commentRevision.CellName = "B2";
                    Console.WriteLine("Modified Cell Location: " + commentRevision.CellName);
                    Console.WriteLine("New Row: " + commentRevision.Row);
                    Console.WriteLine("New Column: " + commentRevision.Column);

                    // Ursprünglichen Zellenamen wiederherstellen
                    commentRevision.CellName = originalCellName;
                }
            }

            // Speichern Sie die Arbeitsmappe mit Revisionen
            workbook.Save("RevisionsClassRevisionCellCommentDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


