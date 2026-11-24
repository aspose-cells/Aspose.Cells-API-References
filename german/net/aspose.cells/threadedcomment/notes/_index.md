---
title: "ThreadedComment.Notes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreadedComment-Eigenschaft. Gibt den Text des Kommentars zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells/threadedcomment/notes/
---
## ThreadedComment.Notes property

Liefert und setzt den Text des Kommentars.

```csharp
public string Notes { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentPropertyNotesDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Einen Autor für ThreadedComment erstellen oder abrufen
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors["User1"];
                author.Name = "User1";

                // Füge einen ThreadedComment zu Zelle A1 (Zeile 0, Spalte 0) mit Anfangstext hinzu
                worksheet.Comments.AddThreadedComment(0, 0, "Initial comment text", author);

                // Den neu hinzugefügten ThreadedComment abrufen
                ThreadedComment threadedComment = worksheet.Comments[0].ThreadedComments[0];

                // Die Notes-Eigenschaft (den Kommentartext) aktualisieren
                threadedComment.Notes = "Updated comment notes";

                // Den Wert der Notes-Eigenschaft lesen und anzeigen
                Console.WriteLine("Threaded comment Notes: " + threadedComment.Notes);

                // Arbeitsmappe speichern (optional)
                workbook.Save("ThreadedCommentNotesDemo.xlsx");
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

* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


