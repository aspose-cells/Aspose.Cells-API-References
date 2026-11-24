---
title: "ThreadedComment.Author"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreadedComment-Eigenschaft. Gibt den Autor des Kommentars zurück"
type: docs
url: /de/net/aspose.cells/threadedcomment/author/
---
## ThreadedComment.Author property

Liefert den Autor des Kommentars.

```csharp
public ThreadedCommentAuthor Author { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyAuthorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Den Standardautor für ThreadedComment aus der Arbeitsmappe abrufen
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                author.Name = "John Doe";
                author.UserId = "john.doe@example.com";

                // Füge einen ThreadedComment zu Zelle A1 (Zeile 0, Spalte 0) hinzu
                worksheet.Comments.AddThreadedComment(0, 0, "Sample comment", author);

                // Den ersten ThreadedComment abrufen
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];

                // Den Wert der Author-Eigenschaft anzeigen (Lesevorgang)
                Console.WriteLine("Author Name: " + comment.Author.Name);
                Console.WriteLine("Author UserId: " + comment.Author.UserId);
                Console.WriteLine("Author ProviderId: " + comment.Author.ProviderId);

                // Demonstrieren Sie das Setzen der Author-Eigenschaft (da sie lesbar/schreibbar ist)
                ThreadedCommentAuthor newAuthor = workbook.Worksheets.ThreadedCommentAuthors[0];
                newAuthor.Name = "Jane Smith";
                newAuthor.UserId = "jane.smith@example.com";
                comment.Author = newAuthor;

                // Zeigen Sie den aktualisierten Wert der Author-Eigenschaft an
                Console.WriteLine("Updated Author Name: " + comment.Author.Name);
                Console.WriteLine("Updated Author UserId: " + comment.Author.UserId);

                // Speichere die Arbeitsmappe
                workbook.Save("ThreadedCommentAuthorDemo.xlsx");
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

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


