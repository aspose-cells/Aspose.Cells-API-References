---
title: "Cell.Comment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Zelleneigenschaft. Gibt den Kommentar dieser Zelle zurück"
type: docs
url: /de/net/aspose.cells/cell/comment/
---
## Cell.Comment property

Liefert den Kommentar dieser Zelle.

```csharp
public Comment Comment { get; }
```

### Hinweise

Wenn kein Kommentar für die Zelle vorhanden ist, wird null zurückgegeben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellPropertyCommentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Einen Kommentar zur Zelle A1 hinzufügen
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Cell");

            // Einen Kommentar zur Zelle hinzufügen
            Comment comment = cell.Comment;
            if (comment == null)
            {
                // Erstelle einen neuen Kommentar, falls keiner existiert
                int commentIndex = worksheet.Comments.Add("A1");
                comment = worksheet.Comments[commentIndex];
                comment.Author = "Author Name";
                comment.Note = "This is a sample comment";
            }

            try
            {
                // Anzeige der Kommentar-Eigenschaften
                Console.WriteLine("Comment Author: " + comment.Author);
                Console.WriteLine("Comment Note: " + comment.Note);
                Console.WriteLine("Comment Row: " + comment.Row);
                Console.WriteLine("Comment Column: " + comment.Column);
                Console.WriteLine("Comment is Visible: " + comment.IsVisible);

                // Einige Kommentar-Eigenschaften ändern
                comment.Note = "Updated comment text";
                comment.IsVisible = true;

                // Aktualisierte Kommentar-Notiz anzeigen
                Console.WriteLine("Updated Comment Note: " + comment.Note);

                // Speichere die Arbeitsmappe
                workbook.Save("CommentDemo.xlsx");
                Console.WriteLine("Comment has been demonstrated and saved to CommentDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Comment](../../comment/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


