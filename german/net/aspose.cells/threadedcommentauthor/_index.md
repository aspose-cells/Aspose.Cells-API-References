---
title: "Klasse ThreadedCommentAuthor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ThreadedCommentAuthor Klasse. Stellt die Person dar, die die Threaded Comments erstellt"
type: docs
url: /de/net/aspose.cells/threadedcommentauthor/
---
## ThreadedCommentAuthor class

Stellt die Person dar, die die Threaded‑Kommentare erstellt.

```csharp
public class ThreadedCommentAuthor
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Name](../../aspose.cells/threadedcommentauthor/name/) { get; set; } | Liest und setzt den Namen. |
| [ProviderId](../../aspose.cells/threadedcommentauthor/providerid/) { get; set; } | Liest die ID des Anbieters. |
| [UserId](../../aspose.cells/threadedcommentauthor/userid/) { get; set; } | Liest und setzt die ID des Benutzers. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassThreadedCommentAuthorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kommentar hinzufügen
            int commentIndex = worksheet.Comments.Add("C1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Initial comment";
            
            // Threaded-Comment-Autoren hinzufügen
            int authorIndex1 = workbook.Worksheets.ThreadedCommentAuthors.Add("Author1", "user1", "");
            ThreadedCommentAuthor author1 = workbook.Worksheets.ThreadedCommentAuthors[authorIndex1];
            
            // Threaded Comment hinzufügen
            int threadedCommentIndex = comment.ThreadedComments.Add("Threaded comment text", author1);
            ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
            
            // Auf den Autor zugreifen und ihn ändern
            Console.WriteLine("Original author: " + threadedComment.Author.Name);
            threadedComment.Author.Name = "ModifiedAuthor";
            Console.WriteLine("Modified author: " + threadedComment.Author.Name);

            // Neuen Autor erstellen und zuweisen
            int authorIndex2 = workbook.Worksheets.ThreadedCommentAuthors.Add("Author2", "user2", "");
            ThreadedCommentAuthor author2 = workbook.Worksheets.ThreadedCommentAuthors[authorIndex2];
            threadedComment.Author = author2;
            Console.WriteLine("New author: " + threadedComment.Author.Name);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


