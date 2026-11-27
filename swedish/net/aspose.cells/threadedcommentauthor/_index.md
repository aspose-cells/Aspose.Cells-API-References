---
title: "Klass ThreadedCommentAuthor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ThreadedCommentAuthor-klass. Representerar personen som skapar de trådade kommentarerna"
type: docs
url: /sv/net/aspose.cells/threadedcommentauthor/
---
## ThreadedCommentAuthor class

Representerar personen som skapar de trådade kommentarerna.

```csharp
public class ThreadedCommentAuthor
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Name](../../aspose.cells/threadedcommentauthor/name/) { get; set; } | Hämtar och anger namnet. |
| [ProviderId](../../aspose.cells/threadedcommentauthor/providerid/) { get; set; } | Hämtar leverantörens id. |
| [UserId](../../aspose.cells/threadedcommentauthor/userid/) { get; set; } | Hämtar och anger användarens id. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassThreadedCommentAuthorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar
            int commentIndex = worksheet.Comments.Add("C1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Initial comment";
            
            // Lägg till trådade kommentarsförfattare
            int authorIndex1 = workbook.Worksheets.ThreadedCommentAuthors.Add("Author1", "user1", "");
            ThreadedCommentAuthor author1 = workbook.Worksheets.ThreadedCommentAuthors[authorIndex1];
            
            // Lägg till en trådad kommentar
            int threadedCommentIndex = comment.ThreadedComments.Add("Threaded comment text", author1);
            ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
            
            // Åtkomst och ändring av författaren
            Console.WriteLine("Original author: " + threadedComment.Author.Name);
            threadedComment.Author.Name = "ModifiedAuthor";
            Console.WriteLine("Modified author: " + threadedComment.Author.Name);

            // Skapa en ny författare och tilldela den
            int authorIndex2 = workbook.Worksheets.ThreadedCommentAuthors.Add("Author2", "user2", "");
            ThreadedCommentAuthor author2 = workbook.Worksheets.ThreadedCommentAuthors[authorIndex2];
            threadedComment.Author = author2;
            Console.WriteLine("New author: " + threadedComment.Author.Name);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


